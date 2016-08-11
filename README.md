# threejsBoxCSG

Simple Box CSG substraction for `THREE.Box3`.

## example: 

```JavaScript
    var b1 = new THREE.Box2(
      new THREE.Vector3(100, 100, 100),
      new THREE.Vector3(200, 200, 200)
    );

    var b2 = new THREE.Box2(
      new THREE.Vector3(10, 50, 100),
      new THREE.Vector3(60, 150, 200)
    );

    var b3 = new THREE.Box2(
      new THREE.Vector3(50, 120, 100),
      new THREE.Vector3(160, 180, 120)
    );

    var b4 = new THREE.Box2(
      new THREE.Vector3(20, 20, 100),
      new THREE.Vector3(140, 80, 120)
    );

    var subtractees = [b1,b2];
    var subtractors = [b3,b4];
    var result      = new BoxCSG(subtractees, subtractors);

    // result = an array of the subtracted boxes that remain
```

![The resulting output](docs/example.png)

- Red: the subtractors
- Blue: the remains of the subtractees

## It also works in 3D

![The 3D example](doc/example3D.png)