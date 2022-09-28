## Phaser
### Scene

- add
  - image
  - graphics 绘几何图
    - clear()
    - fillStyle(color)
    - fillRect(x,y,size,)
  - group
  - sprite(x,y, framekey) 精灵图
    - play(animateKey | {key, repeat})
    - on(event, fn) 监听动画事件(animationrepeat)
    - x 坐标值
  - text(x,y,value,{color})
    - setInteractive()
  - titleSprite()
    - tilePositionX
  
- anims
  - create({key=animatekey, frames=帧, frameRate,yoyo,repeat, repeatDelay}) 创建动画，
  - createFromAseprite(name)
  - generateFrameNames(framekey, {prefix, end, zeroPad})
  - getProgress()
  - on(AnimationsEvents, fn, context)
- input
    - on(gameobjectdown|pointerup, fn)
- load
  - atlas()
  - aseprite(name, path, jsonfile)
  - image()
  - spritesheet()
  - path
  - 
- physics
- tweens
    - addCounter({from, to, duration,delay, ease, repeat, yoy})
    - add({target, x, duration, ease})
    - add({target, props{x{value, ease},y{value, ease}})

### Actions

- PlaceOnCircle(items, gemo)
- RotateAroundDistance(items,{x,y},numaber, value)

### Animations
 - Events
    - ADD_ANIMATION
### Geom

- Circle(x,y,r)