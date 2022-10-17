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
    - on(AnimationsEvents, fn) 监听动画事件(animationrepeat)
    - x 坐标值
  - text(x,y,value,{color})
    - setInteractive()
  - titleSprite()
    - tilePositionX
  
- anims
  - create({key=animatekey, frames=帧, frameRate,yoyo,repeat, repeatDelay}) 创建动画，
  - createFromAseprite(name)
  - generateFrameNames(framekey, {prefix, end, zeroPad})  创建一组Animations.AnimationFrame物件 
  - getProgress() 0到1之间的值，反应当前动画在所有帧中执行的进度


  - on(AnimationsEvents, fn, context)
- input
    - on(gameobjectdown|pointerup, fn)
  
- (load)[https://photonstorm.github.io/phaser3-docs/Phaser.Loader.LoaderPlugin.html]
  - atlas()  打包了一定数量的帧，这些帧有名字索引
  - aseprite(name, path, jsonfile) (Aseprite)[https://www.aseprite.org/]强大的精灵动画编辑器和像素艺术工具
  - image()
  - spritesheet() 添加一个或一组精灵图(精灵图是一张具有准确固定大小的图，里面每个帧都有相同的大小，可以用数字来索引这些帧)
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
    - SPRITE_ANIMATION_START
### Geom

- Circle(x,y,r)