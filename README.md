Hello!

This repository includes the code to our project presented at the UAE GSRC 2023 (This is Noor Odeh speaking!)
Find the abstract below:
https://issuu.com/kubrochures/docs/gsrc_2023_guide_full/18

I wrote most of the code, let me know if you have questions!

Ps. This is the cleaned version of the code, the functional one is more difficult to read; I usually write my codes for my convenience not readability. This one is the opposite though

All parties have approved me doing this, so have at it. The code is free to splice for whoever needs it. Just credit please!

Functionality:
0 - You start by creating a .env file containing your access key from your openAI account
1 - The code first extracts data from an excel sheet that contains templates of expected input-output pairs
هنا بعض الكلام [X1] وما بين الأقواص يمكن ابداله - SQL EXPECTED CODE [X1] MATCHING FEATURE
2 - It then extracts documents containing what the features can be replaced with, the different numbers are there to tell the code which is which
3 - Several random functions determine what details go where. A clause also exists to make sure that all the pairs are unique
4 - After that the data is generated. I usually go for generating about 1k rows, since you're working with a pretrained generator, any more is unnecessary
5 - The data is fed to openAI for preparation and training.
6 - Here I prefer to use a different document with different templates to create the testing data
7 - Testing data is fed to openAI, and a result is retrieved
8 - Rough is used for checking accuracy. Dr. Lamees was the one to recommend this.

I checked the result by hand, and while the 99% accuracy we got was not something I liked, I did not see significant signs of overfitting. Even when writing a few prompts by hand, it still worked pretty well

Best Wishes!
