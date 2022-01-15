<template>
  <div class="control-section">
    <div class="col-lg-9 control-section">
      <ejs-diagram
        style="display: block"
        ref="diagramObj"
        id="diagram"
        :width="width"
        :height="height"
        :snapSettings="snapSettings"
        :rulerSettings="rulerSettings"
        :tool="tool"
      ></ejs-diagram>
    </div>
    <div class="col-lg-3 property-section">
      <div class="property-panel-header">Properties</div>
      <div class="row property-panel-content" id="appearance">
        <div class="row row-header" style="padding-top: 10px">Shapes</div>
        <div class="row" style="padding-top: 8px">
          <div
            title="Retangle"
            class="image-pattern-style e-selected-style"
            id="shape1"
            style="
              background-image: url(./src/diagram/Images/drawingTool/basicshape/DrawingTool_1.png);
              margin-right: 3px;
            "
          ></div>
          <div
            title="Ellipse"
            class="image-pattern-style"
            id="shape2"
            style="
              background-image: url(./src/diagram/Images/drawingTool/basicshape/DrawingTool_2.png);
              margin: 0px 3px;
            "
          ></div>
          <div
            title="Hexagon"
            class="image-pattern-style"
            id="shape3"
            style="
              background-image: url(./src/diagram/Images/drawingTool/basicshape/DrawingTool_3.png);
            "
          ></div>
        </div>
        <div class="row" style="padding-top: 8px">
          <div
            title="Pentagon"
            class="image-pattern-style"
            id="shape4"
            style="
              background-image: url(./src/diagram/Images/drawingTool/basicshape/DrawingTool_4.png);
              margin-right: 3px;
            "
          ></div>
          <div
            title="Polygon"
            class="image-pattern-style"
            id="shape5"
            style="
              background-image: url(./src/diagram/Images/drawingTool/basicshape/DrawingTool_5.png);
              margin: 0px 3px;
            "
          ></div>
          <div
            title="Path"
            class="image-pattern-style"
            id="path"
            style="
              background-image: url(./src/diagram/Images/drawingTool/DrawingTool_6.png);
            "
          ></div>
        </div>
        <div class="row" style="padding-top: 8px">
          <div
            title="Image"
            class="image-pattern-style"
            id="image"
            style="
              background-image: url(./src/diagram/Images/drawingTool/DrawingTool_7.png);
              margin-right: 3px;
            "
          ></div>
          <div
            title="SVG"
            class="image-pattern-style"
            id="svg"
            style="
              background-image: url(./src/diagram/Images/drawingTool/DrawingTool_8.png);
              margin-right: 3px;
            "
          ></div>
          <div
            title="Text"
            class="image-pattern-style"
            id="text"
            style="
              background-image: url(./src/diagram/Images/drawingTool/DrawingTool_9.png);
              margin-right: 3px;
            "
          ></div>
        </div>
        <div class="row row-header" style="padding-top: 10px">Connector</div>
        <div class="row" style="padding-top: 8px">
          <div
            class="image-pattern-style"
            id="straight"
            style="
              background-image: url(./src/diagram/Images/drawingTool/connector/Connectors_1.png);
              margin-right: 3px;
            "
          ></div>
          <div
            class="image-pattern-style"
            id="ortho"
            style="
              background-image: url(./src/diagram/Images/drawingTool/connector/Connectors_2.png);
              margin: 0px 3px;
            "
          ></div>
          <div
            class="image-pattern-style"
            id="cubic"
            style="
              background-image: url(./src/diagram/Images/drawingTool/connector/Connectors_3.png);
            "
          ></div>
        </div>
        <div class="row" style="padding-top: 10px">
          <ejs-checkbox
            id="checked"
            :label="checkedlabel"
            :checked="checkedchecked"
            :change="checkedchange"
          ></ejs-checkbox>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style scoped>
.image-pattern-style {
  background-color: white;
  background-size: 70%;
  background-repeat: no-repeat;
  height: 45px;
  width: calc((100% - 12px) / 3);
  cursor: pointer;
  border: 1px solid #d5d5d5;
  background-position: center;
  float: left;
}

.image-pattern-style:hover {
  border-color: gray;
  border-width: 2px;
}

.row {
  margin-left: 0px;
  margin-right: 0px;
}

.row-header {
  font-size: 12px;
  font-weight: 500;
}

.e-checkbox-wrapper .e-label {
  font-size: 12px;
}

.property-panel-header {
  padding-top: 15px;
  padding-bottom: 5px;
}

.e-selected-style {
  border-color: #006ce6;
  border-width: 2px;
}

.control-section {
  padding-top: 0px;
  padding-bottom: 0px;
  padding-right: 0px;
}

.container-fluid {
  padding-left: 0px;
}

.col-xs-6 {
  padding-left: 0px;
  padding-right: 0px;
}
</style>
