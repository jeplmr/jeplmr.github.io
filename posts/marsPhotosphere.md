---
title: Perseverance Rover Photosphere
description: This time, from Mars!
date: 2021-02-23
tags:
  - Tools
  - Three.JS
  - AR/VR
layout: layouts/post.njk
---

Okay, I know VR photospheres aren't that impressive anymore, but I couldn't resist whipping this one up from the Perseverance rover. Image credit <a href="https://www.jpl.nasa.gov/images/perseverance-navcams-360-degree-panorama" target="blank">JPL</a>.  


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
        map: loader.load('/img/jpegPIA24422_tweakedFOV.jpg'),
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
