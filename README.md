# Salesforce Random Name Generator
A random name generator based on the top 100 last names, top 100 female first names, top 100 male first names. Assists with user acceptance testing when needing large volumes of data in sandboxes, or for demo purposes.

I have found that it is very easy to create tons of fake data for testing configuration or code within sandboxes, or demoing proofs of concepts in production; however, it's trick to create a lot of fake data that actually has meaningful names. I'd prefer to use random data to a spreadsheet with the same names (e.g. presidents, famous people).

Here's the premise of how the **RandomNameGenerator.cls** works:

* Use the list of first names and last names as a starting point
* Multiply the result of Math.random() and the size of the names list, and typecast this as an integer
* Retrieve the first name / last name from the list based on this random integer

## Support & License

Feel free to use this in any way that you would like. If you need help or wish to suggest changes of features, feel free to tweet [@RogerMitchell](https://www.twitter.com/rogermitchell) or add an issue to the repo.