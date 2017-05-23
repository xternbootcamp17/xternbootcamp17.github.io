+++
date = "2017-05-15T11:13:46-04:00"
title = "Day 7: React"
prev="/week2/day6/"
toc = true
weight = 3

+++

<date>Tuesday, May 23, 2017</date>

Combining property initializers and arrow functions also gives us a convenient way to auto-bind `this`:

{{< code jsx >}}
class Something extends React.Component {
  handleButtonClick = (ev) => {
    // `this` is bound correctly!
    this.setState({ buttonWasClicked: true });
  }
}
{{< /code >}}