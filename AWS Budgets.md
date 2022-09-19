# AWS BUDGETS

AWS Budgets is a service use to monitor your AWS costs and usage and take appropriate action. Reserved Instances (RIs) or Savings Plans aggregate utilization and coverage metrics can be tracked using AWS Budgets. It can be used to establish your monthly cost budget with a fixed target amount to keep track of all costs associated with your account.

You can create a monthly cost budget with a variable target amount, with each subsequent month increasing the budget target by 5%. Then, configure your notifications for 80% of your budgeted amount and perform an action. For Instance, you can create an AWS budgets by defining a coverage threshold and then receive notifications when your Savings Plans eligible consumption falls below that threshold. This displays the percentage of your instance usage that is covered by Savings Plans.

## Steps for creating an AWS Budget

1.Firstly you Sign in to the AWS Management Console and then open the AWS Cost Management console at https://console.aws.amazon.com/cost-management/home.

2.Then choose Budgets from the navigation pane.( Below is an image of the Budget Console)

![awsbudgets1](https://user-images.githubusercontent.com/112861600/191072313-72895635-f116-44d3-a881-9a25143caf4d.png)

3.Select Create budget at the top of the page.

4.Choose Cost budget as the budget type. Then select Next.

5.Provide a descriptive name for your budget. Your budget name should be unique and can contain characters, a-z, spaces (eg-Mymonthly-Budget)

6.Choose how often you want the budget to reset the actual and forecasted spend under Set budget amount, Period. You can choose Daily for each day, Montly for each month or Quarterly for every three months, or Annually for each year.Then specify if it would be an expiring budget or recurring budget.

7.Under Budgeting method, choose either a fixed(recommended) or planned. Then enter your budgeted amount(lets say $100)

8.Click All AWS Services under Budget Scope and then click Next.

9.Select your Alert threshhold. You can then choose your threshhold, which can either be a percentage of your budgeted amount(80% in this case), or an absolute value(that is %80)

10.Provide Email recipients you want to notify when the threshold has exceeded(MAXIMUMU OF 10 recipients) and Choose Next.

11.Review your budgets for any errors and then click create. You just created your first AWS Budget. Below is an image of a newly created AWS Budget. 

![Awsbudgets](https://user-images.githubusercontent.com/112861600/191072575-837fb836-3bbd-4d28-a846-9cd3a81906e6.png)
