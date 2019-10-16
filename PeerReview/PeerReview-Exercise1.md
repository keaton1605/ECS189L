# Code Review for Programming Exercise 1 #
## Description ##

For this assignment, you will be giving feedback on the completeness of assignment three: Pikmini. In order to to do so, we will be giving you a rubric to give feedback on. For the feedback, please give positive criticism and suggestions on how to fix segments of code.

You only need to review code modified or created by the student you are reviewing. You do not have to review the code and project files that were given out by the instructor.

Abusive or hateful language or comments will not be tolerated and will result in a grade penalty or be considered a breach of the UC Davis Code of Academic Conduct.

If there are any questions at any point, please email the TA.

Email: zeychen at ucdavis dot edu

## Due Date and Submission Information ##
This code review is due on:
Thursday, October 17th by 11:59 PM

A successful submission should consist of a copy of this markdown document template that is modified with your peer-review. The file name should be the same as it is in the template: PeerReview-Exercise1.md. You also need to include your name and email address in the Peer-reviewer Information section below. This review document should be placed into the base folder of the repo you are reviewing in a branch called review. This branch should be on the origin of the repository you are reviewing.

If you are in the rare situation where there are two peer-reviewers on a single repository, append your UC Davis user name before the extension of your review file. An example: PeerReview-Exercise1-username.md. Both reviewers should submit their reviews in the review branch.  

## Solution Assessment ##

### Description ###

For assessing the solution, you will be choosing ONE choice from: unsatisfactory, satisfactory, good, great, or perfect. Place an x character inside of the square braces next to the appropriate label.

The following are the criteria by which you should assess your peer's solution of the exercise's stages.

#### Perfect #### 
    Can't find any flaws in relation to the prompt. Perfectly satisfied all stage objectives.

#### Great ####
    Minor flaws in one or two objectives. 

#### Good #####
    Major flaw and some minor flaws.

#### Satisfactory ####
    Couple of major flaws. Heading towards solution, however did not fully realize solution.

#### Unsatisfactory ####
    Partial work, not really converging to a solution. Pervasive Major flaws. Objective largely unmet.


### Stage 1 ###

- [x] Perfect
- [ ] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

#### Justification ##### 
Captain moves in the correct direction and with the correct orientation when either movement key is pressed. Code is simple and similar to the movement in opposite direction, and works as intended.

### Stage 2 ###

- [x] Perfect
- [ ] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

#### Justification ##### 
When a pirate is motivated, they will start producing at either a slow, medium, or fast rate and produce for the correct amount of time. Also, the pirates can only be motivated while they are currently exhausted, and attempting to motivate a pirate who is currently producing has no effect. The implementation by waiting PRODUCTION_TIME seconds before producing again is efficient and works well.

### Stage 3 ###

- [x] Perfect
- [ ] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

#### Justifaction ##### 
Has a switch statement which correctly assigns a random work speed to whichever pirate is currently being motivated, with a simple Random.Range() value between 1 and 3. Good implementation of a default case to catch and deal with any errors in the random assignment.

### Stage 4 ###

- [x] Perfect
- [ ] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

#### Justifaction ##### 
Implemented a simple jump command that works as it should, but added complexity with a Serialized field determining how many extra jumps the captain can perform while mid-air. This value works as it, the captain can only jump while they have "extrajumps" remaining, otherwise they must hit the ground before they can jump again. 

## Code Style ##

### Description ###

Good job overall following the style conventions. Comments are in the right places and helpful, and functions are usually clearly seperated and make sense. Variables were correctly named and correctly instanced. There were just a few issues I saw with newlines and spacing:

* [inconsistent newline](https://github.com/ensemble-ai/exercise1-commandpattern-Aligulac/blob/20fdb5e856ac04dd7a5462978516128b51f01dab/Captain/Assets/Scripts/MoveCharacter.cs#L48) - The newlines in this function (MoveCharacterJump) are not necessarily wrong, but they are not consistent with the spacing in the other two functions in this class. 
This also occurs in the worker pirate commands here: 
* [another instance](https://github.com/ensemble-ai/exercise1-commandpattern-Aligulac/blob/20fdb5e856ac04dd7a5462978516128b51f01dab/Captain/Assets/Scripts/FastWorkerPirateCommand.cs#L36)

* [inconsistent spacing](https://github.com/ensemble-ai/exercise1-commandpattern-Aligulac/blob/20fdb5e856ac04dd7a5462978516128b51f01dab/Captain/Assets/Scripts/SlowWorkerPirateCommand.cs#L40) - The spacing between the if and () is different from the other Command functions. Again, this is not wrong, just different from the other template Commands.

## Best Practices ##

### Description ###

This code follows the best practices very well overall. 

* [helpful comments](https://github.com/ensemble-ai/exercise1-commandpattern-Aligulac/blob/20fdb5e856ac04dd7a5462978516128b51f01dab/Captain/Assets/Scripts/CaptainController.cs#L83) - I appreciated how there were comments for all of the new code in the CaptainController to deal with the extra jumps by the Captain. These were placed well to indicate what they referred to, and were succinct while still explaining each new line. These comments should according to conventions be on their own line, but in this case I think the placement makes them more effective.

Aside from a few minor differences, the different classes and functions were all very uniform and easy to understand.

* [well put together functions](https://github.com/ensemble-ai/exercise1-commandpattern-Aligulac/blob/20fdb5e856ac04dd7a5462978516128b51f01dab/Captain/Assets/Scripts/FastWorkerPirateCommand.cs#L30) - The layout and functionality of the different pirate speed commands was very well done. They are easy to follow and work efficiently and the way they are supposed to.

One slight deviation from best practices are certain variable names not being Pascal Case:
* [example of incorrect variable name](https://github.com/ensemble-ai/exercise1-commandpattern-Aligulac/blob/20fdb5e856ac04dd7a5462978516128b51f01dab/Captain/Assets/Scripts/MoveCharacter.cs#L44)

