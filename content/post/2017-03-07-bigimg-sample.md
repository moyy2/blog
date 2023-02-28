---
title: PKL di Mako Brimob
subtitle: jadwal PKL
date: 2017-03-07
tags: ["example", "bigimg"]
bigimg: [{src: "/img/triangle.jpg", desc: "Triangle"}, {src: "/img/sphere.jpg", desc: "Sphere"}, {src: "/img/hexagon.jpg", desc: "Hexagon"}]
---

Masuk pukul 08.00 dan pembelajaran dimulai pukul 09.00 istirahat pukul 12.00 - 14.00 dan pulang pukul 15.00

<!--more-->

A single bigimg can be specified in the front matter by the following YAML:
```
bigimg: [{src: "/img/triangle.jpg", desc: "Triangle"}]
```

Multiple bigimgs can be specified in the front matter by the following YAML:
```
bigimg: [{src: "/img/triangle.jpg", desc: "Triangle"}, 
         {src: "/img/sphere.jpg", desc: "Sphere"}, 
         {src: "/img/hexagon.jpg", desc: "Hexagon"}]
```

Also note that the description field is optional, and images could instead be specified by:
```
bigimg: [{src: "/img/triangle.jpg"}, 
         {src: "/img/sphere.jpg"}, 
         {src: "/img/hexagon.jpg"}]
```

The above YAML array of hashes were written in "flow" style. However when generating a new page or post with `hugo new post/mypost.md`, hugo may interpret the archetype for bigimg in the default YAML style. Defining multiple bigimg's complete with descriptions in this style would be specified by:
```
bigimg: 
- {src: "/img/triangle.jpg", desc: "Triangle"}
- {src: "/img/sphere.jpg", desc: "Sphere"}
- {src: "/img/hexagon.jpg", desc: "Hexagon"}
```

Additional information can be found [in this YAML tutorial](https://rhnh.net/2011/01/31/yaml-tutorial/).