# Use Cases - Workout / Exercise Related

All Use Cases, that are related to Workouts or Exercises

## Add Exercise to Workout

|               | _Add Exercise to Workout_ |
|---------------|---------------------------|
| Description   | Lets Actor add one ore more Exercises to a Workout |
| Actor         | User |
| Pre-condition | Workout must be created |
| Scenario      | 1. Actor is in the view of the Workout </br> 2. System offers various details about the Workout and the Option to add an Exercise to the Workout </br> 3. Actor chooses the Option </br> 4. System offers a list with Exercises </br> 5. Actor can [search](#search-exercise) and select the needed Exercise(s), and then confirm them </br> 6. System adds the Exercise(s) to the Workout |
| Result        | The Exercise(s) are added to the Workout |
| Exceptions    | n/a |
| Extensions    | n/a |

## Create Workout

|               | _Create Workout_ |
|---------------|------------------|
| Description   | Lets Actor create a Workout, which will be used in a Plan |
| Actor         | User |
| Pre-condition | A Plan is already created and has an empty day available |
| Scenario      | 1. Actor is in the View of the Plan </br> 2. System offers various details about the Plan and the Option to create a Workout for a day </br> 3. Actor chooses that Option </br> 4. System asks for information (Unique Name, Day, other Notes) about the Workout </br> 5. Actor provides necessary information </br> 6. System adds Workout to Plan |
| Result        | A new, empty Workout has been added |
| Exceptions    | 2a. All days are already containing Workouts </br> 1. System does not offer the Option to create a Workout </br> 2. Use Case stops </br> 6a. System cannot add the Workout, because the name of the Workout is already in use in the Plan </br> 1. System asks Actor to provide a unique name for the Workout 2. Return to step 5 |
| Extensions    | n/a |

## Search Exercise

|               | _Search Exercise_ |
|---------------|-------------------|
| Description   | Lets Actor search an existing Exercise |
| Actor         | User, Admin |
| Pre-condition | Exercise was [suggested](#suggest-exercise) and [saved](UseCases_Admin.md#review-suggested-exercise) by an Admin |
| Scenario      | 1. Actor enters the view to search an Exercise </br> 2. System offers a list with various Exercises and the ability to filter </br> 3. Actor searches for the Exercise |
| Result        | Actor found the Exercise |
| Exceptions    | 3a. Actor searches for an Exercise that does not exist </br> 1. System shows other Exercises, that conform the applied filters </br> 2. Use Case ends |
| Extensions    | n/a |

## Search Workout

|               | _Search Workout_ |
|---------------|------------------|
| Description   | Lets Actor search an existing Workout |
| Actor         | User, Admin |
| Pre-condition | Workout was [created](#create-workout) and has at least one Exercise [added](#add-exercise-to-workout) |
| Scenario      | 1. Actor enters the view to search a Workout </br> 2. System offers a list with various Workouts and the ability to filter </br> 3. Actor searches for the Workout |
| Result        | Actor found the Workout |
| Exceptions    | 3a. Actor searches for a Workout that does not exist </br> 1. System shows other Workouts that conform the applied filters </br> 2. Use Case ends |
| Extensions    | n/a |

## Set Options of Exercise

|               | _Set Options of Exercise_ |
|---------------|---------------------------|
| Description   | Lets Actor set the Options of an Exercise |
| Actor         | User |
| Pre-condition | Exercise is [added](#add-exercise-to-workout) to a Workout and Actor is in View of Workout |
| Scenario      | 1. Actor selects the Exercise </br> 2. System open the view of the Exercise </br> 3. Actor can change the Options (Sets, Duration, Weight, Reps) and saves |
| Result        | Exercise has been modified |
| Exceptions    | n/a |
| Extensions    | n/a |

## Suggest Exercise

|               | _Suggest Exercise_ |
|---------------|--------------------|
| Description   | Lets Actor suggest an Exercise, which then can be [approved](UseCases_Admin.md#review-suggested-exercise) by an Admin to make it usable in the System |
| Actor         | User |
| Pre-condition | n/a |
| Scenario      | 1. Actor enters the view to suggest an Exercise </br> 2. System offers Options for the Exercise (Name, needed Machines / Weights, Targeted Muscle Groups, other Notes) </br> 3. Actor provides information and saves </br> 4. System shows a summary and asks for confirmation </br> 5. Actor confirms |
| Result        | Exercise has been sent to an Admin |
| Exceptions    | 4a. Actor provides not enough information </br> 1. System informs Actor that more information are needed </br> 2. Return to step 3 |
| Extensions    | n/a |

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