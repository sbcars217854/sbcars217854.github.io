[Back](https://sbcars217854.github.io/)

# Manual Validation

For the manual validation, we selected a set of 96 commits, split by the 7 different projects we analyzed, and then further split into 5 groups: 2 groups relating to our findings 3 and 4, 1 group exploring other interactions between refactorings and other factors, one for Low Decay classes, plus one for High Decay classes. 

This led to an average of 15 commits per project (as some projects did not have commits that fit in a specific subcategory/finding).

To execute the validation the 3 participants (one PhD and two graduate students) were each given a single code change per project per subcategory and had access to the following information: the hash of the commit containing the change, its contents, the specific file in which the rules were found, and the tags for that change. From that information, they had to describe, where possible, the intent of the developer when performing those changes, as well as if (and how) they relate to one of the findings in the paper. 

In summary, from the results, we were able to see that -- for Finding 3 -- 12 out of 21 commits were directly related to the finding itself, while most of the other 9 commits were "tangentially" related (a refactoring occurred together with another non-refactoring change that caused decay). For finding 4, 12 out of 15 commits were directly related to the finding itself, with the other 3 commits being unrelated to the finding (but not contradicting it). Finally, from the refactoring group, 2 non-related commits were found due to false positives in the refactoring detection.

The spreadsheet that was used for the manual validation can be downloaded **[here](https://github.com/sbcars217854/sbcars217854.github.io/blob/main/replication_package/manual_validation/manual_validation.xlsx?raw=true)**. 