---
title: Simple ThreeJS VR-Enabled Photosphere
description: VR Enabled this time!
date: 2021-02-14
tags:
  - Tools
  - Three.JS
  - AR/VR
layout: layouts/post.njk
---

Okay, I think I've got a basic handle on ThreeJS now. This one is pretty simple. It's just a scene with a single sphere mesh that has a photoshere texture assigned to its material. Oh, and I'm drawing backfaces, too. For some reason I can't get this to run in FireFox, but Edge works just fine? I'll look into it. Tested with Edge and a Quest 2 via Oculus Link. 


<canvas id="c" style="width:100%; height:100%; text-align: center"></canvas>
<script type="module">

import * as THREE from 'https://threejsfundamentals.org/threejs/resources/threejs/r125/build/three.module.js';
import {VRButton} from 'https://threejsfundamentals.org/threejs/resources/threejs/r125/examples/jsm/webxr/VRButton.js';

function main() {
  const canvas = document.querySelector('#c');
  const renderer = new THREE.WebGLRenderer({canvas});
  renderer.xr.enabled = true;
  document.body.appendChild(VRButton.createButton(renderer));

  const fov = 75;
  const aspect = 2;  // the canvas default
  const near = 0.1;
  const far = 16;
  const camera = new THREE.PerspectiveCamera(fov, aspect, near, far);
  camera.position.set(0, 1.6, 0);

  const scene = new THREE.Scene();


    const radius = 12; 
    const widthSegments = 24; 
    const heightSegments = 24; 
    const sphere = new THREE.SphereGeometry(radius, widthSegments, heightSegments); 

    const loader = new THREE.TextureLoader();
    const material = new THREE.MeshBasicMaterial({
        map: loader.load('/img/PHOTOSPHERE.jpg'),
        side: THREE.DoubleSide, 
    });

    const bgMesh = new THREE.Mesh(sphere, material);
    scene.add(bgMesh);
    bgMesh.position.set(0, 0, 0); 


  function resizeRendererToDisplaySize(renderer) {
    const canvas = renderer.domElement;
    const width = canvas.clientWidth;
    const height = canvas.clientHeight;
    const needResize = canvas.width !== width || canvas.height !== height;
    if (needResize) {
      renderer.setSize(width, height, false);
    }
    return needResize;
  }

  function render(time) {
    time *= 0.001;

    if (resizeRendererToDisplaySize(renderer)) {
      const canvas = renderer.domElement;
      camera.aspect = canvas.clientWidth / canvas.clientHeight;
      camera.updateProjectionMatrix();
    }

    renderer.render(scene, camera);
  }

  renderer.setAnimationLoop(render);
}

main();

</script>
