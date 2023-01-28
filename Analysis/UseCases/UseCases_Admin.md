# Use Cases - Admin related

All Use Cases, that are related to an Admin of the System:
  - Delete Exercise ([O](#delete-exercise))
  - Delete Plan ([O](#delete-plan))
  - Review reported plan ([O](#review-reported-plan))
  - Review suggested Exercise ([O](#review-suggested-exercise))

## Delete Exercise

|               | _Delete Exercise_ |
|---------------|-------------------|
| Description   | Lets Actor delete an Exercise |
| Actor         | Admin |
| Pre-condition | Exercise needs to be [searched](UseCases_WE.md#search-exercise) by Actor |
| Scenario      | 1. Actor opens the details of the Exercise </br> 2. System offers various details for that Exercise and the Option to delete the Exercise </br> 3. Actor chooses that Option </br> 4. System asks for confirmation </br> 5. Actor confirms |
| Result        | Exercise has been deleted and cannot be searched or included in Workouts |
| Exceptions    | n/a |
| Extensions    | n/a |

## Delete Plan

|               | _Delete Plan_ |
|---------------|---------------|
| Description   | Lets Actor delete a Plan |
| Actor         | Admin |
| Pre-condition | Plan needs to be [searched](UseCases_Plan.md#search-plan) by Actor |
| Scenario      | 1. Actor opens the details of the Plan </br> 2. System offers various details of that Plan and an Option to delete the Plan </br> 3. Actor chooses that Option </br> 4. System asks for confirmation </br> 5. Actor confirms |
| Result        | Plan has been deleted and cannot be searched |
| Exceptions    | n/a |
| Extensions    | n/a |

## Review reported Plan

|               | _Review reported Plan_ |
|---------------|---------------|
| Description   | Lets Actor review a Plan |
| Actor         | Admin |
| Pre-condition | Plan was [reported](UseCases_Plan.md#report-plan) by at least one User |
| Scenario      | 1. Actor opens the Report </br> 2. System shows the Plan and the Reason why the Plan was reported while also showing Options to delete the Report or delete the Plan </br> 3. Actor chooses to [delete the Plan](#delete-plan) |
| Result        | Report was reviewed and handled |
| Exceptions    | n/a |
| Extensions    | 3a. Actor chooses to delete the Report </br> 1. Report was deleted, while the Plan is untouched </br> 2. Use Case ends |

## Review Suggested Exercise

|               | _Review Suggested Exercise_ |
|---------------|-----------------------------|
| Description   | Lets Actor review an Exercise, which was suggested by a User |
| Actor         | Admin |
| Pre-condition | There is a [suggested Exercise](UseCases_WE.md#suggest-exercise) |
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