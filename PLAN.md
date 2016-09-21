# Planning Basketball ScoreKeeper App

## Model

TODO: Model's Shape

```haskell
Model =
  { players : List Player
  , playerName : String
  -- If the player has an Id, we knwo were in Edit mode, otherwise add mode
  , playerId : Maybe Int
  , plays : List Play
  }
```

TODO: Player Shape
```
  Player =
  {   id : Int
    , name : String
    , points : Int

  }
```

TODO: Play Shape
```
  Play =
  {
    , name : String
    , playerId : Int
    , points: Int
  }
```

TODO: Modes
```
Edit Player
Add Player
Have to keep track of which mode it is all in
```

TODO: Initial Model
```
initModel : Model
initModel =
```

## Update

What can be done in our App

* Edit
* Score
* Input
* Save
* Cancel
* DeletePlay

TODO: Create message union type for each of the 6 actions

TODO: Create update function(s) that'll handle all 6 actions

## View

What are the logial sections of our UI?

* main view (outermost function): will be passed to the HTML
  * title
  * player section
    * player list header
    * player list
      * player
    * player total
  * player form
  * play section
    * play list header
    * play list
      * play

TODO: Create functions for each of the above sections
