# Frontend-assessment - Searchable Select List

## Overview

We'd like you to create a searchable select list that retrieves characters from the [Marvel api](https://developer.marvel.com/docs#!/public/getCreatorCollection_get_0).

The style and behaviour of the select list should match the images shown below.

### Request

To retrieve a list of characters:

`GET http://localhost:1111/characters`

To query for characters by their name:

`GET http://localhost:1111/characters?nameStartsWith=iron`

### Response

A simplified response can be seen below. The name, description and thumbnail properties are required for this assessment.

```json
{
  "results": [
    {
      "id": "1",
      "name": "Iron Man",
      "description": "Wounded, captured and forced to build a weapon by his enemies, billionaire industrialist Tony Stark instead created an advanced suit of armor to save his life and escape captivity. Now with a new outlook on life, Tony uses his money and intelligence to make the world a safer, better place as Iron Man.",
      "thumbnail": {
        "path": "http://i.annihil.us/u/prod/marvel/i/mg/9/c0/527bb7b37ff55",
        "extension": "jpg"
      }
    }
  ]
}
```

## Mandatory Requirements

- Cannot use third party search select library
- Behaviour and style should be the same as shown in the images below
- Items in the list should be selectable via a mouse click. On select, the character name should be written to the console.
- A loader should be shown when the results are being queried from the API

## Examples

Mobile Example 1 - Closed Select
![ScreenShot4](https://i.imgur.com/KUaenjW.jpg)

Mobile Example 2 - Opened Select
![ScreenShot5](https://i.imgur.com/KAJvi1s.jpg)

Mobile Example 3 - No Results Select
![ScreenShot6](https://i.imgur.com/0938RCR.jpg)
