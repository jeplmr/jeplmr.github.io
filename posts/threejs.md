---
title: ThreeJS Tinkering
description: JavaScript strikes again...
date: 2021-02-13
tags:
  - Tools
  - Three.JS
layout: layouts/post.njk
---

I'm tinkering with ThreeJS, expect some jank. A lot of jank.


<canvas id="c" style="width:100%; height:100%"></canvas>
<script type="module">

import * as THREE from "https://threejsfundamentals.org/threejs/resources/threejs/r125/build/three.module.js";

function main(){
    const canvas = document.querySelector('#c');
    const renderer = new THREE.WebGLRenderer({canvas});

    const fov = 90; 
    const aspect = 2;  // the canvas default
    const near = 0.1;
    const far = 5;

    const camera = new THREE.PerspectiveCamera(fov, aspect, near, far);
    camera.position.z = 2.5;

    const scene = new THREE.Scene();

    const boxWidth = 1;
    const boxHeight = 1;
    const boxDepth = 1;
    const geometry = new THREE.BoxGeometry(boxWidth, boxHeight, boxDepth);

    const material = new THREE.MeshPhongMaterial({color: 0x44aa88});  // greenish blue
  
    const color = 0xFFFFFF;
    const intensity = 1;
    const light = new THREE.DirectionalLight(color, intensity);
    light.position.set(-1, 2, 4);
    scene.add(light);


    
    function makeInstance(geometry, color, x) {
        const material = new THREE.MeshPhongMaterial({color});
      
        const cube = new THREE.Mesh(geometry, material);
        scene.add(cube);
      
        cube.position.x = x;
      
        return cube;
    }

    const cubes = [
        makeInstance(geometry, 0x44aa88,  0),
        makeInstance(geometry, 0x8844aa, -2),
        makeInstance(geometry, 0xaa8844,  2),
    ];

    function render(time) {
        time *= 0.001;  // convert time to seconds
      
        cubes.forEach((cube, ndx) => {
            const speed = 1 + ndx * .1;
            const rot = time * speed;
            cube.rotation.x = rot;
            cube.rotation.y = rot;
        });
      
        renderer.render(scene, camera);
        renderer.setSize( screen.width/2, screen.height/2 );
      
        requestAnimationFrame(render);
      }
      requestAnimationFrame(render);
}

main();

</script>
