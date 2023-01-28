# Use Cases - Account related

All Use Cases, that are related to the Account:
  - Create Account ([O](#create-account))
  - Log in ([O](#log-in))
  - Log out ([O](#log-out))
  - Open created Workouts ([O](#open-created-workouts))
  - Open saved Plans ([O](#open-saved-plans))

## Create Account

|               | _Create Account_ |
|---------------|------------------|
| Description   | Lets Actor create an Account to use the System |
| Actor         | User |
| Pre-condition | Actor is not logged in |
| Scenario      | 1. Actor chooses the Option for creating an Account </br> 2. System asks for necessary information about the Actor (Username, E-Mail, Password, Birthdate, Focus of Training) </br> 3. Actor provides information and saves them </br> 4. System displays given information and asks if these are correct </br> 5. Actor confirms </br> 6. System creates Account and logs into Account |
| Result        | Actor has created an Account that can be then used |
| Exceptions    | 3a. Actor does not give all necessary information </br> 1. System informs Actor that not all information are given </br> 2. Return to step 3 |
| Extensions    | 5a. Actor does not confirm </br> 1. System returns to window where the information can be inputted </br> 2. Return to step 2 |

## Log in

|               | _Log in_ |
|---------------|----------|
| Description   | Lets Actor log into their Account to make use of the System |
| Actor         | User |
| Pre-condition | Actor is not logged in and has an Account |
| Scenario      | 1. Actor chooses the Option to  log in </br> 2. System asks for E-Mail and Password </br> 3. Actor provides information </br> 4. System checks the given information </br> 5. When valid information is given, System logs into the Account |
| Result        | Actor has access to all Account details and the System functions |
| Exceptions    | 5a. Information is not valid </br> 1. System informs Actor that the given information is not valid </br> 2. Return to step 3 |
| Extensions    | n/a |

## Log out

|               | _Log out_ |
|---------------|-----------|
| Description   | Lets Actor log out of their Account, which then makes the Actor not being able to use the System |
| Actor         | User |
| Pre-condition | Actor is [logged in](#log-in) |
| Scenario      | 1. Actor opens the Account details </br> 2. System offers many actions for the Account </br> 3. Actor chooses to log out </br> 4. System asks for confirmation </br> 5. Actor confirms </br> 6. System logs Actor out |
| Result        | Actor has not access to Account and cannot use the System |
| Exceptions    | n/a |
| Extensions    | n/a |

## Open created Workouts

|               | _Open created Workouts_ |
|---------------|-------------------------|
| Description   | Lets Actor open the list of their created Workouts |
| Actor         | User |
| Pre-condition | n/a |
| Scenario      | 1. Actor opens the list of their created Workouts </br> 2. System shows a list with all of their created Workouts while also giving the Option to [search a Workout](UseCases_WE.md#search-workout) |
| Result        | List has been opened |
| Exceptions    | n/a |
| Extensions    | 2a. Actor has not created any Workouts </br> 1. System informs the Actor that the Actor has not created Workouts yet </br> 2. Use Case ends |

## Open saved Plans

|               | _Open saved Plans_ |
|---------------|---------------|
| Description   | Lets Actor open the list of their saved Plans |
| Actor         | User |
| Pre-condition | n/a |
| Scenario      | 1. Actor opens the list of their saved Plans </br> 2. System shows a list with all of their saved Plans while also giving the Option to [search a Plan](UseCases_Plan.md#search-plan) |
| Result        | List has been opened |
| Exceptions    | n/a |
| Extensions    | 2a. Actor has not saved any Plans </br> 1. System informs the Actor that the Actor has not saved Plans yet </br> 2. Use Case ends |

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