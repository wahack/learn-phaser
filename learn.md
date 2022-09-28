### 资源预加载preload

> this.load.[method]

- spritesheet加载游戏物件的雪碧图(name, path, {frameWdith: number, frameHeight: number}) 

- atlas 加载游戏物件图鉴(比spritesheet更复杂的雪碧图,并有对应的包含各个物体位置/大小json文件


### 添加游戏物件

> this.add

- group 构建物件池

    ```
      A Group is a way for you to create, manipulate, or recycle similar Game Objects.
      Group membership is non-exclusive. A Game Object can belong to several groups, one group, or none.
      Groups themselves aren't displayable, and can't be positioned, rotated, scaled, or hidden.

    ```


    group(options)构造函数，返回group对象
    
    group对象的方法
    
    - create(x,y,key,frame) 往组里添加一个新物件



### Actions

- IncX(items, value)  给每个物件的x属性加上值value
- IncY 同IncX
- Rotate(items, value) 给每个物件的rotate属性加上值value
- GridAlign(items, config) 将物件按配置排列到网格



### Animations

anims.create({
  key: '', frames: , frameRate: number, yoyo: bool, repeat: -1, repeatDelay: 300
})