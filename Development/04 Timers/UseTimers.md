- You can use Timers to execute asynchronous logic in your OutSystems application.

-  This is useful to execute batch tasks like sending emails at a predetermined time, or to execute logic to configure an application after its deployment.


## How Timers Are Handled

- Timers are handled by the OutSystems Scheduler Service. This service checks for Timers that are ready to run and executes their actions. A Timer is ready to run when the current time is greater or equal to the Timer runtime property NextRun.

- The timeout of a Timer is set by default to 20 minutes, but you can change it by setting the Timeout in Minutes property of the timer.


###### Asynchronous logic, such as Timers and Process Activities, run in a separate session. All session variables will start with their default value when executing an action associated with a timer or process activity.

## Force the Timer to run


There are two ways of forcing a Timer to run without waiting for the scheduled time:

- Using the Wake<Timer Name> built-in action
- Running the Timer in Service Center