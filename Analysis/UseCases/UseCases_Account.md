# Use Cases - Account related

All Use Cases, that are related to the account

## Create account

|               | _Create account_ |
|---------------|------------------|
| Description   | Lets actor create an account to use the system |
| Actor         | User |
| Pre-condition | Actor is not logged in |
| Scenario      | 1. Actor clicks the designated button for creating an account </br> 2. System asks for necessary information about the actor </br> 3. Actor provides all information and saves them </br> 4. System displays given information and asks if these are correct </br> 5. Actor confirms </br> 6. System creates account and logs into account |
| Result        | Actor has created an account that can be then used |
| Exceptions    | 3a. Actor does not give all necessary information </br> 1. System informs actor that not all information are given </br> 2. Return to step 3 |
| Extensions    | 5a. Actor does not confirm </br> 1. System returns to window where the information can be inputted </br> 2. Return to step 2 |

## Log in

|               | _Log in_ |
|---------------|----------|
| Description   | Lets actor log into their account to make use of the system |
| Actor         | User |
| Pre-condition | Actor is not logged in and has an account |
| Scenario      | 1. Actor clicks on the specified log in-button </br> 2. System asks for E-Mail and password </br> 3. Actor provides information </br> 4. System checks the given information </br> 5. When valid information is given, system logs into the account |
| Result        | Actor has access to all account details and the system functions |
| Exceptions    | 5a. Information is not valid </br> 1. System informs actor that the given information is not valid </br> 2. Return to step 3 |
| Extensions    | n/a |

## Log out

|               | _Log out_ |
|---------------|-----------|
| Description   | Lets actor log out of their account, which then makes the actor stop using the system |
| Actor         | User |
| Pre-condition | Actor is [logged in](#log-in) |
| Scenario      | 1. Actor opens the account details </br> 2. System offers many actions for the account </br> 3. Actor chooses to log out </br> 4. System asks for confirmation </br> 5. Actor confirms </br> 6. System logs actor out |
| Result        | Actor has not access to account and cannot use the system |
| Exceptions    | n/a |
| Extensions    | 5a. Actor does not confirm </br> 1. System closes dialog </br> 2. Actor still has access their account and can continue using the system </br> 3. Use Case stops|

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