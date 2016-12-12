# CardShow

CardShow is a jQuery plugin of drawing cards.


## Options

- __src__: ```String``` 抽奖用户数据，根据需要生成
- __autoDrawing__: ```Boolean``` 自动抽取/手动抽取，默认为 true（自动抽）
- __backface__: ```Boolean``` 卡片入场是否背面显示，默认为 true（背面显示）
- __rows__: ```Number``` 卡片分几行显示，建议最大值为 3
- __drawingCardsNum__: ```Number``` 每轮次抽取的卡片数，默认为 1 张
- __drawingRounds__: ```Number``` 抽奖轮次，默认为 0（不限次）
- __drawingSpeed__: ```Number``` 自动抽取的速度，默认为 300

## Usage

### html:
```html
<ul class="card-container card-perspective">
	<li class="card card-flip">
	    <figure class="card-front">
	        <img src="img/1.jpg"/>
	        <figcaption>about</figcaption>
	    </figure>
	    <div class="card-back"></div>
	</li>
</ul>
```

### instance:
```js
var cs = $('.card-container').cardshow({
	         src: data,
	         autoDrawing: true,
	         backface: true,
	         rows: 1,
	         drawingCardsNum: 3,
	         drawingRounds: 0,
	         drawingSpeed: 300
	     });
```


## Demo

[https://nzbin.github.io/CardShow](https://nzbin.github.io/CardShow)

## License

MIT License

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
