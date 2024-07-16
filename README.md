# Grow-grub 🌱

## Overview

Grow-grub is a full-stack companion app for gardeners that was made as my final group project at Dev Academy. It was built over the course a week in a team of six other students. 

The application allows users to plan their garden and track the progress of their plants. Users can get a wealth of information about their plants such as care instructions and advice on when to sow and harvest. The application also tracks the watering history of each plant and generates a new watering task depending on the current date, when the plant was last watered, and the watering frequency of the plant. 

The application is currently functional and I am currently working on hosting and deploying it. However, we were coding right up until code freeze and haven't touched the codebase since, so there are lots of comments and other errata that still need to be cleaned up!

## My technical contribution

We started work on Grow-grub after I had worked on [TableTalk](https://github.com/cburkeg/TableTalk) (a front-end-heavy project), so I wanted to further develop my skills on the back-end during this project. 

### Back-end
#### I worked on the following [routes](server/routes/growGrub.ts):

- [Saving a new garden](server/routes/growGrub.ts#L195) (please note that didn't write lines relating to saving plants, e.g. line 204, lines 206 - 211)
- [Updating an existing garden](server/routes/growGrub.ts#L233) (please note that I didn't write line 255 onwards)
- [Refreshing and retrieving user tasks](server/routes/growGrub.ts#L313)
- [Completing a task](server/routes/growGrub.ts#L344)

#### I also worked on the following [database functions](server/db/growGrub.ts):

- [saveNewGarden](server/db/growGrub.ts#L101)
- [saveNewPlots](server/db/growGrub.ts#L113)
- [updateGardenLayout](server/db/growGrub.ts#L135)
- [getPlotsPlantsJoinByAuth](server/db/growGrub.ts#L385)
- [getUncompletedTasksByAuth](server/db/growGrub.ts#L405)
- [updateTasks](server/db/growGrub.ts#L434)
- [createTasks](server/db/growGrub.ts#L450)
- [getUpdatedTasksByAuth](server/db/growGrub.ts#L416)
- [completeTask](server/db/growGrub.ts#L457)

#### Finally, I wrote the following [helper functions](server/db/helperFunctions.tsx):
- [differentiatePlots](server/db/helperFunctions.tsx#L10)
- [refreshTasks](server/db/helperFunctions.tsx#L75)
 

### Front-end

I helped code the [GardenGrid](client/components/GardenGrid.tsx) and [GardenForm](client/components/GardenGrid.tsx) components along with the [GardenView](client/pages/GardenView.tsx) page.

## Other contributions

I was our team's scrum facilitator. It was my responsibility to organise our stand-ups, make sure our group project was tracking smoothly, and resolve roadblocks from the team's workflow. I also helped facilitate our retro at the end of the week-long project. 
