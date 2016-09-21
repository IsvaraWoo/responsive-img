###This is a wrapper for [responsive-images.js](https://github.com/kvendrik/responsive-images.js).


###Installation
```sh
npm install --save responsive-img
```

###Usage
####More info please check [responsive-images.js](https://github.com/kvendrik/responsive-images.js).

####Use with webpack
Require it like other library:
```js
require('responsive-img');
```

####Use with react
1. Should config data-src according [responsive-images.js](https://github.com/kvendrik/responsive-images.js) guide.
2. Manully call makeImagesResponsive once. usually call it on componentDidMount is a good choice. 
```js
var Box = React.createClass({
  componentDidMount: function () {
    ...
    makeImagesResponsive(this.refs.box);
  },
  render: function () {
    return (
      <div ref="box">
        <img data-src={'<960:' + require('../img/960.jpg') + ',>960:' + require('../img/1200.jpg')} />
      </div>
    );
  }
});
```

###Comments
Let me know if you have idea’s or notice something, I would love to hear your feedback!
