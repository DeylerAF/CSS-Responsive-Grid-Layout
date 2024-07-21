# CSS Responsive Grid Layout

## Try it out here: https://deyleraf.github.io/CSS-Responsive-Grid-Layout/

![Alt text](assets/CSSGridLayout.gif)

## Desktop Layout
```css
.container {
  display: grid;
  grid-template-rows: 80px auto 1fr auto 50px;
  grid-template-columns: 1fr 4fr 1fr;
  height: 100vh;
  grid-template-areas:
    "header        header        header"
    "left-aside    banner        right-aside"
    "left-aside    main          right-aside"
    "left-aside    low-content   right-aside"
    "footer        footer        footer";
  grid-gap: 10px;  padding: 10px;
  font-weight: 600;  font-size: 20px;
}
```

## Mobile Layout
```css
@media (max-width: 678px) {
.container {
  grid-template-rows: 50px 50px 50px 1fr 
  50px 50px 50px;
  grid-template-columns: 1fr;
  grid-template-areas:
    "header"
    "banner"
    "left-aside"
    "main"
    "right-aside"
    "low-content"
    "footer";
  }
}
```