# tags-input-react

Tags Input Component

## How to Install

Make sure you have [Node.js](http://nodejs.org/) and NPM installed.

```sh
npm install tags-input-react
```

## Demo

Check demo online [here](http://santhosh.pro/projects#tags-input).

## How to Use

```sh
import React, { Component } from 'react'
import TagsInput from 'tags-input-react'

class TagsInputDemo extends Component {
  constructor() {
    super()
    this.state = {
      tags: []
    }
    this.handleOnChange = this.handleOnChange.bind(this)
  }

  handleOnChange (tags, value) {
    this.setState({
      tags
    })
  }

  render() {
    return (
      <TagsInput
        placeholder='Type here...'
        onChange={this.handleOnChange}
      />
    )
  }
}
```

## Available PropTypes

| Prop Name | Type | Default Value | Description |
| --- | --- | --- | --- |
| tags | array | [] | Array of tags for Pre-populate in Input|
| preventDuplicates | Boolean | true | Preventing duplicates in tags |
| placeholder | string | 'Type here' | Placeholder in input |
| onChange | Function | null | Callback function to get the tags created by user |