## Light & Camera

### Lights

* [ambientLight()](http://processingjs.org/reference/ambientLight_/)
* [directionalLight()](http://processingjs.org/reference/directionalLight_/)
* [lightFalloff()](http://processingjs.org/reference/lightFalloff_/)
* [lightSpecular()](http://processingjs.org/reference/lightSpecular_/)
* [lights()](http://processingjs.org/reference/lights_/)
* [noLights()](http://processingjs.org/reference/noLights_/)
* [normal()](http://processingjs.org/reference/normal_/)
* [pointLight()](http://processingjs.org/reference/pointLight_/)
* [spotLight()](http://processingjs.org/reference/spotLight_/) : Note - on this linked page, this function's syntax is `spotLight(v1, v2, v3, nx, ny, nz, angle, concentration)`, which SHOULD BE `spotLight(v1, v2, v3, x, y, z, nx, ny, nz, angle, concentration)`

### Camera

* [beginCamera()](http://processingjs.org/reference/beginCamera_/)
* [camera()](http://processingjs.org/reference/camera_/)
* [endCamera()](http://processingjs.org/reference/endCamera_/)
* [frustum()](http://processingjs.org/reference/frustum_/)
* [ortho()](http://processingjs.org/reference/ortho_/)
* [perspective()](http://processingjs.org/reference/perspective_/)
* [printCamera()](http://processingjs.org/reference/printCamera_/)
* [printProjection()](http://processingjs.org/reference/printProjection_/)

### Coordinates

* [modelX()](http://processingjs.org/reference/modelX_/)
* [modelY()](http://processingjs.org/reference/modelY_/)
* [modelZ()](http://processingjs.org/reference/modelZ_/)
* [screenX()](http://processingjs.org/reference/screenX_/)
* [screenY()](http://processingjs.org/reference/screenY_/)
* [screenZ()](http://processingjs.org/reference/screenZ_/)

### Material Properties

* [ambient()](http://processingjs.org/reference/ambient_/)
* [emissive()](http://processingjs.org/reference/emissive_/)
* [shininess()](http://processingjs.org/reference/shininess_/)
* [specular()](http://processingjs.org/reference/specular_/)

### Example

```python
from processing import *

def setup():
    size(560, 400, P3D)
    #printCamera()
    #printProjection()

def draw():
    noFill()
    beginCamera()
    camera()
    rotateX(-PI/6)
    endCamera()

    translate(50, 50, 0)
    rotateY(PI/3)
    box(45)


run()
```

### Reference

* [Processingjs](http://processingjs.org/reference/)