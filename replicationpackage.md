[Back](https://sbcars217854.github.io/)

# Data Set

## File Change History

**Format:** csv

**Fields:** 
* **change_id**: String used to identify a change throughout the entire dataset. It is in the following format `<FILE_NUMBER>_change<NUMBER>`. Changes are numbered in reverse chronological order, i.e. `change1` always represents the most recent modification to a file. 
* **commit_hash:** Git identification hash used to reference a commit.
* **current_path:** Path where the file currently resides.
* **old_path:** If the file was moved in that change (or created in that change, when value is `None`), it is the previous path where the file used to be located. If the file wasn't moved, it equals `current_path`.

**Observations**: N/A

**[Download Link](https://github.com/sbcars217854/sbcars217854.github.io/tree/main/replication_package/file_changes)**

## File Changes with Metrics

**Format:** csv

**Fields:** 
* **change_id**: String used to identify a change throughout the entire dataset. It is in the following format `<FILE_NUMBER>_change<NUMBER>`. Changes are numbered in reverse chronological order, i.e. `change1` always represents the most recent modification to a file. 
* **commit_hash:** Git identification hash used to reference a commit.
* **current_path:** Path where the file currently resides.
* **old_path:** If the file was moved in that change (or created in that change, when value is `None`), it is the previous path where the file used to be located. If the file wasn't moved, it equals `current_path`.
* **PercentLackOfCohesion:** LCOM (Software Metric)
* **CountClassCoupled:** CBO (Software Metric)
* **MaxNesting:** MaxNEST (Software Metric)
* **SumCyclomatic:** Sum Cyclomatic Complexity (Software Metric)
* **SumCyclomaticModified:** Sum Modified Cyclomatic Complexity (Software Metric)
* **SumCyclomaticStrict:** Sum Strict Cyclomatic Complexity (Software Metric)
* **SumEssential:** Sum Essential Complexity (Software Metric)
* **AvgCyclomatic:** Average Cyclomatic Complexity (Software Metric)
* **AvgCyclomaticModified:** Average Modified Cyclomatic Complexity (Software Metric)
* **AvgCyclomaticStrict:** Average Strict Cyclomatic Complexity (Software Metric)
* **AvgEssential:** Average Essential Complexity (Software Metric)
* **CountDeclMethod:** Local Methods (Software Metric)
* **MaxCyclomatic:** Max Cyclomatic Complexity (Software Metric)
* **MaxCyclomaticModified:** Max ModifiedCyclomatic Complexity (Software Metric)
* **MaxCyclomaticStrict:** Max Strict Cyclomatic Complexity (Software Metric)
* **MaxEssential:** Max Essential Complexity (Software Metric)
* **CountLine:** Physical Lines (Software Metric)
* **CountLineBlank:** Blank LOC (Software Metric)
* **CountLineCode:** LOC (Software Metric)
* **CountLineCodeDecl:** Declarative Lines of Code (Software Metric)
* **CountLineCodeExe:** Executable Lines of Code (Software Metric)
* **CountLineComment:** CLOC (Software Metric)
* **CountSemicolon:** Semicolons (Software Metric)
* **CountStmt:** Statements (Software Metric)
* **CountStmtDecl:** Declarative Statements (Software Metric)
* **CountStmtExe:** Executable Statements (Software Metric)
* **RatioCommentToCode:** Comment to Code Ratio (Software Metric)
* **CountDeclInstanceVariable:** NIV (Software Metric)
* **CountDeclInstanceMethod:** NIM (Software Metric)
* **CountDeclMethodAll:** RFC - Response for Class (Software Metric)
* **CountDeclMethodDefault:** Local Default Visibility Methods (Software Metric)
* **AvgLine:** Average Number of Lines (Software Metric)
* **AvgLineBlank:** Average Number of Blank Lines (Software Metric)
* **AvgLineCode:** Average Number of Lines of Code (Software Metric)
* **AvgLineComment:** Average Number of Lines with Comments (Software Metric)
* **CountDeclClassMethod:** Class Methods (Software Metric)
* **CountDeclClassVariable:** Class Variables (Software Metric)
* **CountDeclMethodPrivate:** Private Methods (Software Metric)
* **CountDeclMethodProtected:** Protected Methods (Software Metric)
* **CountDeclMethodPublic:** Public Methods (Software Metric)
* **CountClassBase:** IFANIN (Software Metric)
* **CountClassDerived:** NOC (Software Metric)
* **MaxInheritanceTree:** DIT (Software Metric)
* **TightClassCohesion:** TCC (Software Metric)
* **FANOUT:** FANOUT (Software Metric)
* **FANIN:** FANIN (Software Metric)
* **LCOM2:** LCOM2 (Software Metric)
* **LCOM3:** LCOM 3 (Software Metric)
* **ChangeSet:** Change Set (Process-related metric)
* **HunksCount:** Hunks Count (Process-related metric)
* **CodeChurn:** Code Churn (Process-related metric)
* **ContributorCount:** Contributor Count (Developer-related metric)
* **FileContributionPercentage:** File Contribution Percentage (Developer-related metric)
* **RefactoringCount:** Total Number of Refactorings (Process-related metric)
* **MoveRefactoringCount:** Number of Move Refactorings (Process-related metric)
* **ExtractionRefactoringCount:** Number of Extraction Refactorings (Process-related metric)
* **HierarchicalRefactoringCount:** Number of Hierarchical Refactorings (Process-related metric)
* **RenameRefactoringCount:** Number of Rename Refactorings (Process-related metric)
* **num_pulls_classes:** Number of Associated Pull-Requests (Developer-related metric)
* **words_in_discussion_by_class:** Number of Words in Discussion (Developer-related metric)
* **words_per_comment_by_class:** Number of Words per Comment (Developer-related metric)

**Observations**: This file contains additional metrics which weren't used in the analysis presented in the paper.

**[Download Link](https://github.com/sbcars217854/sbcars217854.github.io/tree/main/replication_package/file_changes_with_all_metrics)**

## Decay Score

**Format:** csv

**Fields:** 
* **file_id**: Integer that identifies a file throughout the whole dataset.
* **decay_score**: Score, ranging from 0 to 1, that was calculated for each file. More details in step 5 of section III.B of the paper.

**Observations**: N/A

**[Download Link](https://github.com/sbcars217854/sbcars217854.github.io/tree/main/replication_package/decay_score)**

## Tagged Changes

**Format:** csv

**Fields:** 
* **change_id**: String used to identify a change throughout the entire dataset. It is in the following format `<FILE_NUMBER>_change<NUMBER>`. Changes are numbered in reverse chronological order, i.e. `change1` always represents the most recent modification to a file. 
* **tags**: List of tags (divided by the `|` character) that were attributed to each change. More details in Step 7 of section III.B.

**Observations**: N/A

**[Download Link](https://github.com/sbcars217854/sbcars217854.github.io/tree/main/replication_package/tagged_changes)**

## Association Rules

**Format:** csv

**Fields:** 
* **Items**: All tags present in the association rule.
* **Antecedents**: Antecedents for the association rule.
* **Consequent**: Consequents for the association rule.
* **Support**: Support metric.
* **Confidence**: Confidence metric.
* **Lift**: Lift metric.

**Observations**: Separated into two csvs for each project. They are named `<PROJECT>_low` for rules inferred from slightly-decayed classes and `<PROJECT>_high` for ones inferred from largely-decayed classes.

**[Download Link](https://github.com/sbcars217854/sbcars217854.github.io/tree/main/replication_package/association_rules)**

## Summarized Rules

**Format:** csv

**Fields:** 
* **items**: All tags present in the association rule.
* **antecedents**: Antecedents for the association rule.
* **consequent**: Consequents for the association rule.
* **support_low**: Support metric.
* **support_high**: Support metric.
* **confidence_low**: Confidence metric.
* **confidence_high**: Confidence metric.
* **lift_low**: Lift metric.
* **lift_high**: Lift metric.

**Observations**: Since these csvs aggregate the association rules from both rules, the support, confidence and lift metrics are split. They are named `<METRIC>_low` when inferred from slightly-decayed classes and `<METRIC>_high` when inferred from largely-decayed classes.

**[Download Link](https://github.com/sbcars217854/sbcars217854.github.io/blob/main/replication_package/summarized_rules)**