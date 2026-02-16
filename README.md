[responsive-canvas](https://dirkarnez.github.io/responsive-canvas)
==================================================================
FROM [HTML5 canvas... responsive! - DEV Community](https://dev.to/georgedoescode/html5-canvas-responsive-2keh)

### Notes
- DO NOT hand-write responsive-canvas
  - Use [dirkarnez/pixijs-webgl-playground](https://github.com/dirkarnez/pixijs-webgl-playground) where pixijs already provides responsive and `window.devicePixelRatio`-supporting canvas, and we can use yoga-layout inside pixijs
    - ```javascript
      await app.init({
        antialias: true, // Enable antialiasing
        resolution: window.devicePixelRatio, // Screen resolution
        preference: 'webgl', // 'webgl' or 'webgpu'
        background: '#1099bb', 
        resizeTo: window,
        autoResize: true,
        autoDensity: true
      });
      ```
### TODOs
- [ ] make it a library

### Based on
- [Three.js - Responsive HD-DPI](https://threejs.org/manual/examples/responsive-hd-dpi.html)
  - [Responsive Design - three.js manual](https://threejs.org/manual/#en/responsive)
- [szimek/signature_pad: HTML5 canvas based smooth signature drawing](https://github.com/szimek/signature_pad)
  - https://szimek.github.io/signature_pad/js/app.js
- [molstar/src/mol-canvas3d/util.ts at master · molstar/molstar](https://github.com/molstar/molstar/blob/master/src/mol-canvas3d/util.ts)
- [autoscale-canvas/index.js at master · component/autoscale-canvas](https://github.com/component/autoscale-canvas/blob/master/index.js)
- [hughsk/canvas-autoscale: A variant of canvas-fit that handles some extra magic for you: adjusting the scale of the canvas to maintain smooth framerates](https://github.com/hughsk/canvas-autoscale)
- [webgpu-samples/sample/resizeCanvas/main.ts at main · webgpu/webgpu-samples](https://github.com/webgpu/webgpu-samples/blob/main/sample/resizeCanvas/main.ts)
- [tldraw/tldraw: very good whiteboard SDK / infinite canvas SDK](https://github.com/tldraw/tldraw)
- [Responsive Canvas Stage Demo | Konva - JavaScript Canvas 2d Library](https://konvajs.org/docs/sandbox/Responsive_Canvas.html)
- https://github.com/theacodes/kicanvas/blob/main/src/graphics/canvas2d.ts
- [surfer-project / surfer · GitLab](https://gitlab.com/surfer-project/surfer)
  - App UI
