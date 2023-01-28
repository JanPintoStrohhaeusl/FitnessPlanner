# Use Cases - Admin related

All Use Cases that are related to an Admin of the System 

## Delete Exercise

|               | _Delete Exercise_ |
|---------------|-------------------|
| Description   | Lets Actor delete an Exercise |
| Actor         | Admin |
| Pre-condition | Exercise needs to be [searched](UseCases_WE.md#search-exercise) by Actor |
| Scenario      | 1. Actor opens the details of the exercise </br> 2. System offers various details for that exercise and a button to delete the exercise </br> 3. Actor clicks on that button </br> 4. System asks for confirmation </br> 5. Actor confirms |
| Result        | Exercise has been deleted and cannot be searched or included in Workouts |
| Exceptions    | n/a |
| Extensions    | n/a |

## Delete Plan

|               | _Delete Plan_ |
|---------------|---------------|
| Description   | Lets Actor delete a Plan |
| Actor         | Admin |
| Pre-condition | Plan needs to be searched by Actor |
| Scenario      | 1. Actor opens the details of the plan </br> 2. System offers various details of that plan and a button to delete the plan </br> 3. Actor clicks on that button </br> 4. System asks for confirmation </br> 5. Actor confirms |
| Result        | Plan has been deleted and cannot be searched |
| Exceptions    | n/a |
| Extensions    | n/a |

## Review Suggested Exercise

|               | _Review Suggested Exercise_ |
|---------------|-----------------------------|
| Description   | Lets Actor review an Exercise, which was suggested by a User |
| Actor         | Admin |
| Pre-condition | There is a suggested Exercise |
| Scenario      | 1. Actor opens the view to see suggested Exercises </br> 2. System offers a list with suggested Exercises </br> 3. Actor selects one Exercise </br> 4. System shows all the details of that Exercise </br> 5. Actor saves that Exercise </br> 6. System asks for confirmation </br> 7. Actor confirms |
| Result        | Exercise is saved into the System and can be searched and used in Workouts |
| Exceptions    | n/a |
| Extensions    | 5a. Actor rejects that Exercise </br> 1. System asks for confirmation </br> 2. Actor confirms |

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