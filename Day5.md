# Day5

DevOps framework  | CI/CD--CD=> Continous Delivery —Plan ->Code -> Build -> Test
CI => Continuous Integration  — Deploy -> Operate -> Monitor
￼
The DevOps process begins with planning, it is advisable that the Devops engineer be involved in the planning  of a development sprint. 

## Plan

It all starts with the planning process this is where the development team gets together and figure out what types of features and bug fixes that they're going to roll out in their next sprint. This is an opportunity as a DevOps Engineer for you to get involved with that and learn what kinds of things are going to be coming your way that you need to be involved with and also influence their decisions or their path and kind of help them work with the infrastructure that you've built or steer them towards something that's going to work better for them in case they're not on that path and so one key thing to point out here is the developers or software engineering team is your customer as a DevOps engineer so this is your opportunity to work with your customer before they go down a bad path.

## Code

Now once that planning session's done they're going to go start writing the code you may or may not be involved a whole lot with this one of the places you may get involved with it, is whenever they're writing code you can help them better understand the infrastructure so if they know what services are available and how to best talk with those services so they're going to do that and then once they're done they'll merge that code into the repository

## Build

This is where we'll kick off the first of our automation processes because we're going to take their code and we're going to build it depending on what language they're using it may be transpiling it or compiling it or it might be creating a docker image from that code either way we're going to go through that process using our ci cd pipeline

## Testing

Once we've built it we're going to run some tests on it now the development team usually writes the test you may have some input in what tests get written but we need to run those tests and the testing is a way for us to try and minimise introducing problems out into production, it doesn't guarantee that but we want to get as close to a guarantee as we can that were one not introducing new bugs and two not breaking things that used to work

## Release

Once those tests pass we're going to do the release process and depending again on what type of application you're working on this may be a non-step. You know the code may just live in the GitHub repo or the git repository or wherever it lives but it may be the process of taking your compiled code or the docker image that you've built and putting it into a registry or a repository where it's accessible by your production servers for the deployment process

## Deploy

which is the thing that we do next because deployment is like the end game of this whole thing because deployments when we put the code into production and it's not until we do that that our business actually realizes the value from all the time effort and hard work that you and the software engineering team have put into this product up to this point.

## Operate

Once it's deployed we are going to operate it and operate it may involve something like you start getting calls from your customers that they're all annoyed that the site's running slow or their application is running slow right so you need to figure out why that is and then possibly build auto-scaling you know to handle increase the number of servers available during peak periods and decrease the number of servers during off-peak periods either way that's all operational type metrics, another operational thing that you do is include like a feedback loop from production back to your ops team letting you know about key events that happened in production such as a deployment back one step on the deployment thing this may or may not get automated depending on your environment the goal is to always automate it when possible there are some environments where you possibly need to do a few steps before you're ready to do that but ideally you want to deploy automatically as part of your automation process but if you're doing that it might be a good idea to include in your operational steps some type of notification so that your ops team knows that a deployment has happened

## Monitor

All of the above parts lead to the final step because you need to have monitoring, especially around operational issues auto-scaling troubleshooting like you don't know there's a problem if you don't have monitoring in place to tell you that there's a problem so some of the things you might build monitoring for are memory utilization CPU utilization disk space, api endpoint, response time, how quickly that endpoint is responding and a big part of that as well is logs. Logs give developers the ability to see what is happening without having to access production systems.

** Still editing though
