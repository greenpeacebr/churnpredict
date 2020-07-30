# Machine Learning For Good 
This project was started at 12/2019, at this event representing GPBR I could receive consulting from professionals of the field. It's a classification model that attempts to predict if a Regular Giving is likely to be cancelled in the near future, so that we can apply engagement routines to the Donor thus preventing fundraising loss.

## How does it work?

This is a classification model, it'll receive Regular Giving Data from a given Donor and will classify that as True or False to be likely to get cancelled.

First I had to extract and clean the data from our platform and since we have a peculiar political scenario I've decided to use only Regular Givings that were active after our presidential impeachment. Finishing the process I ended with around 72k Regular Givings Lines to feed the ML model.

From the Regular Giving object I've chosen these features:

- Age
- Gender
- Installments
- Value
- Payment Method
- Welcome Call (Received or not)
- Welcome Pack (Received or not)

Comment: With these features I could get around 82% accuracy, but these can be discussed and of course the model can be tunned in many ways, changing the features is something I heavily consider.

Finally we can use pickle or joblib (Python Packages) to serve this model at our local API. One of way using it is to run a batch job at Salesforce with a given Rule, to categorize active Regular Givings as in "Churn" or not, the ones that are marked as True must receive some sort of engagement communication and that is to be discussed with other areas of the organization.

## Things to improve

Theres plenty of things to improve, from code readability to the decisions on the model itself, before getting here I've attempted many other types of models and was pretty much just studying the subject, after almost a year and much coding I know it's far from being ready to go. But it's something I'm willing to work on if it's going to be deployed.