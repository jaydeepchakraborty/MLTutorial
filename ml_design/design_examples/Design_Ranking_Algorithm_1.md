# Ranking Algorithm

<ul>
    <li>
        <b>Step 1 - Problem Statement :</b> <br>
        &rarr;  What is the goal of the experiment ?
        <ul>
            Step 1.1 - Business Goal :
            <ul>
                You want to introduce new ranking algorithm to provide more relevant products to customers.
            </ul>
        </ul>
        <ul>
            Step 1.2 - Stakeholder/ User Journey : 
            <ul>
                End User Activity -> <br>
                visit --> search item --> [Browse item] --> views item --> purchase
            </ul>
        </ul>
        <ul>
            Step 1.3 - Success Metric : (Measurable, Effective, Sensitive, Timely)
            <ul>
                Revenue per day per user
            </ul>
        </ul>
    </li>
    <li>
        <b> Step 2 - Hypothesis Testing : </b> <br>
        &rarr; What result you hypothesize from the experiment ?
        <ul>
            Step 2.1 - Hypothesis Statements
            <ul>
                &rarr; Null Hypothesis (H_0): <br>
                The avg revenue per day per user between the baseline and variant ranking 
                algorithms are same.
            </ul>
            <ul>
                &rarr; Alternative Hypothesis (H_a): <br>
                The avg revenue per day per user between the baseline and variant ranking 
                algorithms are different.
            </ul>
        </ul>
        <ul>
            Step 2.2 - Significance Level (Alpha)
            <ul>
                Alpha = 0.05 (Prob(Type I error))
                if p-value is less than Alpha, then reject H_0
            </ul>
        </ul>
        <ul>
            Step 2.3 - Statistical Power
            <ul>
                Statistical Power = 0.80 <br>
                The probability of detecting an effect if H_a is true
            </ul>
        </ul>
        <ul>
            Step 2.4 - Minimum detectable effect (MDE)
            <ul>
                MDE = 1% (for million of users)<br>
                If the changes is at-least 1% higher in revenue per day per user then it is practically significant.
            </ul>
        </ul>
    </li>
    <li>
        <b> Step 3 - Design the Experiment : </b> <br>
        &rarr; what are the experiment parameters ?
        <ul>
             Step 3.1 - Set the randomization Unit (target gp, control gp) <br>
            &rarr; On whom or what we do the A/B test
            <ul>
                Randomization Unit: User
            </ul>
        </ul>
        <ul>
            Step 3.2 - Target Population
            <ul>
                Visitors who searches the product
            </ul>
        </ul>
        <ul>
            Step 3.3 - sample size
            <ul>
                n ~ 
            </ul>
        </ul>
        <ul>
            Step 3.4 - Duration of the experiment
            <ul>
                1 - 2 weeks
            </ul>
        </ul>
    </li>
    <li>
        <b> Step 4 - Run the Experiment : </b> <br>
        &rarr; What are requirements for running the experiment ?
    </li>
    <li>
        <b> Step 5: Validity Checks : </b> <br>
        &rarr; Did the experiment run without erros or bias
        <ul>
            Instrumentation Effect
            <ul>
                Guardrail metric - latency time
            </ul>
        </ul>
        <ul>
            External Factors
            <ul>
                Holidays, Economic disruption (e.g Covid)
            </ul>
        </ul>
        <ul>
            Selection Bias
            <ul>
                A/A test
            </ul>
        </ul>
        <ul>
            Sample Ratio mismatch
            <ul>
                chi-square goodness for fit test
            </ul>
        </ul>
        <ul>
            Novelty Effect
            <ul>
                segment by new and old visitors
            </ul>
        </ul>
    </li>
    <li>
        <b> Step 6 - Interpret Result :  </b> <br>
        &rarr; The direction of the hypothesis and metric significance
    </li>
    <li>
        <b> Step 7: Launch Decision :  </b> <br>
        &rarr; Based on the results and trade-offs, should we launch ?
        <ul>
            sd
        </ul>
    </li>
</ul>

<ul>
    Resources: 
    <li>
        https://www.youtube.com/watch?v=DUNk4GPZ9bw
    </li>
    <li>
        https://www.youtube.com/watch?v=DUNk4GPZ9bw
    </li>
</ul>