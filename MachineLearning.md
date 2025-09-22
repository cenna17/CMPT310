# Learning from Examples - Chatper 19 Up to 19.7.2

## Forms of Learning

`Induction` = specific set of observ. -> general rule

`Factored Representation` = a list (vector) of features/values of something

`Regression` = Where the output for the set of inputs is a `number`

`Classification` = Where the output for the set of inputs is a bunch of stuff that can be divided or 'classified'

`Attributes` = the features which define a test case.  (ie. Apples attributes: sour taste, red/green exterior, large etc)

### Supervised Learning

- Is directed; we give things labels (usually as part of testing set) and try to get the machine to give the correct label for new things/inputs

- We give it feedback (right guess/wrong guess)

- Test (input) and predictions (output) of the models can be graphed using polynomial functions.

#### 
`Hypothesis space` - the set of all possible models/functions a ML algo. can choose from to learn a relationship between input data and output predictions.

* We may use a (polynomial) function to 'fit' the models predictions to the actual outcomes that we are looking for.

* The model may build a `hypotheses - h` and we say that the hypothesis `generalize` well if it can accurately predict outputs given some set of test cases.

    - `Underfitting` - when the model fails to find a pattern in the data

    - `Overfitting` - when the model pays too much attention to the particular data set its trained on => failed/poor predictions when given unseen data.

            => These 'new' data may be completely different from the tests its seen previously or ONLY SOMEWHAT DIFFERENT

### Unsupervised Learning  

- Not directed; we DO NOT give it feedback

- Tasks: clustering (detect clusters of cases that may become usefull)

### Reinforcement Learning

- Learning from reward and punishment

### Learning Decision Trees

* The model tries to reach for a resultby asking a series of questions.  With each Q&A towards the test case, it leads the model 'down' the tree and 'across' branches until it reaches a conclusion/preiction about the test csae at a leaf node.

** In general, outputs can be discrete/continuous.  For now we consider the output to be BOOLEAN -> `T/F -> [+]/[-] output results only`

    *** The nodes at each branch represents a yes/no answer, dividing up test cases across the branches as we filter down the decision tree.

    **** How do we know the decision of the model at a branch is correct?

        - `Entropy` measures the uncertainty of a random variable

            `more info -> less entropy` // makes sense consider the more we know the more there is to go on

            `we're absolutely sure` -> entropy is zero (eg. the sun always rises in the east)
        
        - `Random Variable (V) 

    Prob. of uncertainty (entropy) of a random variable is: 
    
    ![By equation](imgs/eqn-entropy.png)

