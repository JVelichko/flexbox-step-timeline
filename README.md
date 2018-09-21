# flexbox-step-timeline
Step timeline component is written in SCSS using flexbox and can be used for adaptive cross browser layout. The component is supported at least by the following browsers: Firefox 50+, Google Chrome 59+, Safari 10+, IE 11+, Edge. It has two styles: dotted and lined.

## Usage

 For basic usage you need to create structure as show in example below.
 Pug example:
```pug
.timeline-step.dotted
        .step.past
          span.marker
          span.title Step 1
        .step.past
          span.marker
          span.title Step 2
        .step.current
          span.marker
          span.title Step 3
        .step.future
          span.marker
          span.title Step 4
```

Pug transforms the above to HTML:


```html
<div class="timeline-step dotted">
  <div class="step past">
    <span class="marker"></span>
    <span class="title">Step 1</span>
  </div>
  <div class="step past">
    <span class="marker"></span>
    <span class="title">Step 2</span>
  </div>
  <div class="step current">
    <span class="marker"></span>
    <span class="title">Step 3</span>
  </div>
  <div class="step future">
    <span class="marker"></span>
    <span class="title">Step 4</span>
  </div>
</div>
```

## Dotted timeline

Labels are aligned in the center of the check-points. In this case, the first and the last has left and right alignment, respectively. Labels can be placed both above and below the timeline.

![Dotted timeline](https://i.imgur.com/M5iRtmo.jpg)

Pug:

```pug
.timeline-step.dotted.up
        .step.past
          span.marker
          span.title Step 1
        .step.past
          span.marker
          span.title Step 2
        .step.current
          span.marker
          span.title Step 3
        .step.future
          span.marker
          span.title Step 4
```

HTML:

```html
<div class="timeline-step dotted up">
  <div class="step past">
    <span class="marker"></span>
    <span class="title">Step 1</span>
  </div>
  <div class="step past">
    <span class="marker"></span>
    <span class="title">Step 2</span>
  </div>
  <div class="step current">
    <span class="marker"></span>
    <span class="title">Step 3</span>
  </div>
  <div class="step future">
    <span class="marker"></span>
    <span class="title">Step 4</span>
  </div>
</div>
```

## Lined timeline

Labels are aligned in the center of progress line. Labels can be placed both above and below the timeline.
Don't include label to the last step. Four steps timeline will have 4 progress lines and 5 check-points.

![Lined timeline](https://i.imgur.com/nGD2yYd.jpg)

Pug:

```pug
.timeline-step.lined
        .step.past
          span.marker
          span.title step 1
        .step.past
          span.marker
          span.title step 2
        .step.current
          span.marker
          span.title step 3
        .step.future
          span.marker
          span.title step 4
        .step.future
          span.marker
```

HTML:

```html
<div class="timeline-step lined">
  <div class="step past">
    <span class="marker"></span>
    <span class="title">Step 1</span>
  </div>
  <div class="step past">
    <span class="marker"></span>
    <span class="title">Step 2</span>
  </div>
  <div class="step current">
    <span class="marker"></span>
    <span class="title">Step 3</span>
  </div>
  <div class="step future">
    <span class="marker"></span>
    <span class="title">Step 4</span>
  </div>
  <div class="step future">
    <span class="marker"></span>
  </div>
</div>
```

## Demo

See [demo](https://codepen.io/julijuly4/pen/KxJaZL) on CodePen 
