# Issue 1:
**Description:** The ComingSoon component is named exported from the file, but it has been imported as a default import.
**Impact:** The ComingSoon component cannot be found in the app.js file.
**Solution:** Export the ComingSoon component as default from the component.

# Issue 2:
**Description:** The ComingSoon component function is in camelCase, but the convention is to use PascalCase for component names.
**Impact:** This approach can mix up HTML tags and React components.
**Solution:** Use PascalCase for the ComingSoon component.

# Issue 3:
**Description:** The remaining variable in the clockInterval function gives negative time counting.
**Impact:** Users won't understand if time is remaining or already passed.
**Solution:** Set the date in the end variable in future time than past or current time to solve the issue.

# Issue 4:
**Description:** The end date is being calculated every one second as the end variable is defined inside the clockInterval function.
**Impact:** Recalculating a static value doesn't make sense.
**Solution:** Set the end variable outside the clockInterval function scope to its parent scope.

# Issue 5:
**Description:** The code continues to calculate time even after the end time has already passed.
**Impact:** Users won't understand what is happening as the time is still counting rather than stopping.
**Solution:** Check if the current timestamp is greater than the end timestamp. If true, clear the interval and return to not run the below code.

# Issue 6:
**Description:** The validate email function isn't working properly.
**Impact:** It can't detect wrong email.
**Solution:** Rewrite the validate function with the test prototype method of regex.

# Issue 7:
**Description:** While invoking the hitToast function, the argument list isn't in the right order.
**Impact:** HitToast function is producing an error.
**Solution:** Alter the argument sequence while invoking the hitToast function.