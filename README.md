# React Goblin Builder App

**Visit the live demo here:** [Live Demo](https://sad-pike-d255ed.netlify.app/)

| User should be able to . . .                                                         |             |
| :----------------------------------------------------------------------------------- | ----------: |
| Visit the deployed app on Netlify, with link in the About section of the Github repo |  **required for grading** |

| Events                                                                                |             |
| :----------------------------------------------------------------------------------- | ----------: |
| On changing the goblin form, the current goblin item updates |        .5 |
| On submitting the goblin form, a new goblin is added to the view  |        1 |
| On clicking a goblin the goblin gets deleted  |        .5 |
| On typing in the filter input, the goblins are filtered by name  |        1 |

| Components                                                                                |             |
| :----------------------------------------------------------------------------------- | ----------: |
| `App()` : tracks state for `allGoblins`,  `filteredGoblins`, `goblinFormName`, `goblinFormHP`, `goblinFormColor` |.5|
| `App()` : passes state as props correctly to `GoblinForm`, `Goblin`, and `GoblinList` |.5|
| `App()` : define a `submitGoblin` function that adds a new goblin to the array using form state. Note that this function gets passed down to the goblin form, which is where it will be attached to a submit listener |1|
| `App()` : define a `handleDeleteGoblin` function that deleted a goblin from the state array using id |1|
| `App()` : define a `handleFilterGoblins` function that takes in a string and set `filteredGoblins` to an array of goblins whose name matches that string |1|
| `GoblinForm({ setGoblinFormName, goblinFormName, setGoblinFormHP, goblinFormHP, setGoblinFormColor, goblinFormColor, submitGoblin })` : on change for each input, call the appropriate state handler prop with the correct `e.target.value` to update `App.js` state.  |1|
| `GoblinForm({ setGoblinFormName, goblinFormName, setGoblinFormHP, goblinFormHP, setGoblinFormColor, goblinFormColor, submitGoblin })` : on submit, add a goblin to state by calling `props.submitGoblin` in the correct way.  |1|
| `GoblinList({ goblins, handleDeleteGoblin })` : takes in a `goblins` prop and renders a list of `Goblin` components. Note the prop drilling with `handleDeleteGoblin` |.5|
| `Goblin({ goblin, handleDeleteGoblin })` : takes in a goblin and renders it with the correct color background. Note the prop drilling with `handleDeleteGoblin` |.5|

## Stretch goal ideas:
- Note that the delete functionality doesn't work if the filter is active. Why is that? Can you fix it?
- Track the `query` as state. Use `useEffect` to filter the goblins every time this query changes.
- 
![image](https://user-images.githubusercontent.com/16160135/150245997-20e6bcfd-53da-4243-a484-a0153f9638b4.png)
