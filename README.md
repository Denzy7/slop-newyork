# Slop New York

A New York City simulation built with [three.js](https://threejs.org/), WebGPURenderer, and TSL. Explore Manhattan on foot, by car, by bicycle, or by helicopter.

[Try it live](https://denzy7.github.io/slop-newyork/)

This is a fork of [mrdoob/slop-newyork](https://github.com/mrdoob/slop-newyork) ([live demo of the original](https://mrdoob.github.io/slop-newyork/)) that makes it playable on low-end GPUs and browsers without WebGPU:

- A graphics settings menu (gear button): resolution, shadows, reflections, antialias, draw distance and city detail, saved per browser.
- A low-tier profile when WebGPU is unavailable and three.js falls back to WebGL 2: lighter defaults and a cheaper "City detail: Low" path (simpler facades, fewer far buildings, trees and traffic).
- Frustum culling for the Manhattan facade boxes, and fixes for the crowds and instanced meshes on WebGL 2.

To run it locally, serve the folder over http (not `file://`), e.g. `python3 -m http.server 8000`, and open http://localhost:8000.

## Make it your own

Fork it, remix it, improve it, break it. Make games, animations, films, experiments, or something completely different. Use it as a starting point and take it wherever you want. Have fun!

## License and data

The project code is available under the [MIT License](LICENSE).

Geographic data: NYC Open Data and © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright) (ODbL). Third-party data and dependencies retain their respective licenses.
