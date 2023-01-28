# Use Cases - Plan related

All Use Cases, that are related to a Plan:
  - Add Workout to Plan ([O](#add-existing-workout-to-plan))
  - Create Plan ([O](#create-plan))
  - Report Plan ([O](#report-plan))
  - Save Plan ([O](#save-plan))
  - Search Plan ([O](#search-plan))

## Add existing Workout to Plan

|               | _Add existing Workout to Plan_ |
|---------------|---------------|
| Description   | Lets Actor add an existing Workout to a Plan |
| Actor         | User |
| Pre-condition | Workout must [contain at least one Exercise](UseCases_WE.md#add-exercise-to-workout), Actor needs to be Owner of the Plan and Plan needs to have at least one day unoccupied |
| Scenario      | 1. Actor opens the view of the Plan </br> 2. System offers all details of the Plan and the Option to add a Workout for a specific day </br> 3. Actor chooses that Option </br> 4. System asks if the Workout is a Workout that has been created by the Actor or is a Workout that has been created by someone else </br> 5. Actor chooses the first Option </br> 6. System shows a list with all by the Actor created Workouts and gives the Ability to [search the Workout](UseCases_WE.md#search-workout) </br> 7. Actor chooses a Workout |
| Result        | Workout has been added |
| Exceptions    | 3a. Plan does not have a day unoccupied </br> 1. System informs Actor that there are no days left </br> 2. Use Case ends |
| Extensions    | 5a. Actor chooses the second Option </br> 1. System shows a list with all public Workouts and gives the ability to [search the Workout](UseCases_WE.md#search-workout) </br> 2. Actor chooses a Workout </br> 3. Use Case ends |

## Create Plan

|               | _Create Plan_ |
|---------------|---------------|
| Description   | Lets Actor create a Plan |
| Actor         | User |
| Pre-condition | n/a |
| Scenario      | 1. Actor chooses to create a Plan </br> 2. System asks for information (Name, Visibility, other Notes) </br> 3. Actor provides information </br> 4. System creates Plan |
| Result        | An empty Plan has been and can be filled with Workouts |
| Exceptions    | n/a  |
| Extensions    | n/a |

## Report Plan

|               | _Report Plan_ |
|---------------|---------------|
| Description   | Lets Actor reports a Plan |
| Actor         | User |
| Pre-condition | n/a |
| Scenario      | 1. Actor opens the view of the Plan </br> 2. System offers all details of the Plan and the Option to report the Plan </br> 3. Actor chooses that Option </br> 4. System asks for the reason </br> 5. Actor provides the reason </br> 6. System sends the Report to an Admin |
| Result        | Plan has been reported |
| Exceptions    | n/a |
| Extensions    | n/a |

## Save Plan

|               | _Save Plan_ |
|---------------|-------------|
| Description   | Lets Actor save a Plan |
| Actor         | User |
| Pre-condition | Plan must be visible to Actor (Public / Created by Actor) |
| Scenario      | 1. Actor opens the view of the Plan </br> 2. System offers all details of the Plan and the Option to save the Plan </br> 3. Actor chooses that Option |
| Result        | Plan has been saved |
| Exceptions    | 3a. Plan has already been saved </br> 1. System informs Actor that the Plan has already been saved to their Account </br> 2. Use Case ends |
| Extensions    | n/a |

## Search Plan

|               | _Search Plan_ |
|---------------|---------------|
| Description   | Lets Actor search a Plan |
| Actor         | User |
| Pre-condition | Plan must be visible to Actor (Public / Created by Actor) |
| Scenario      | 1. Actor enters the view to search a Plan </br> 2. System offers a list with various Plans and the ability to filter </br> 3. Actor searches for the Plan |
| Result        | Actor found the Plan |
| Exceptions    | 3a. Actor searches for a Plan that does not exist </br> 1. System shows other Plans, that conform the applied filters </br> 2. Use Case ends |
| Extensions    |  |

### Table template

|               | _UseCaseName_ |
|---------------|---------------|
| Description   |  |
| Actor         |  |
| Pre-condition |  |
| Scenario      |  |
| Result        |  |
| Exceptions    |  |
| Extensions    |  |