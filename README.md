# react-slick

### I added noRightPadding's API in Settings for empty space at the end.

### Example

```js
import React from "react";
import Slider from "react-slick";

class VariableWidth extends React.Component {
  render() {
    const settings = {
      className: "slider variable-width",
      dots: true,
      infinite: false,
      slidesToShow: 3,
      slidesToScroll: 3,
      variableWidth: true,
      noRightPadding: true,
    };
    return (
      <div
        style={{
          margin: "0 50px",
          padding: "0 30px",
          border: "1px solid gray ",
        }}
      >
        <h2>Variable width</h2>
        <Slider {...settings}>
          <div style={{ width: 100 }}>
            <p>100</p>
          </div>
          <div style={{ width: 200 }}>
            <p>200</p>
          </div>
          <div style={{ width: 75 }}>
            <p>75</p>
          </div>
          <div style={{ width: 300 }}>
            <p>300</p>
          </div>
          <div style={{ width: 225 }}>
            <p>225</p>
          </div>
          <div style={{ width: 175 }}>
            <p>175</p>
          </div>
          <div style={{ width: 220 }}>
            <p>220</p>
          </div>
          <div style={{ width: 111 }}>
            <p>111</p>
          </div>
          <div style={{ width: 180 }}>
            <p>180</p>
          </div>
          <div style={{ width: 210 }}>
            <p>210</p>
          </div>
        </Slider>
      </div>
    );
  }
}
```
