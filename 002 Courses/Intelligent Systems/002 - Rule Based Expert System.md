Tags: #RuleBasedExpertSystem #IntellgientSystem 

**Expert System**: a computer program that contains expert knowledge about a particular problem, often in the form of a set of if-then rules, that is able to solve problems at a level equivalent or greater than human experts.

**Building Expert System**: To transfer expertise from human experts to a computer system and then on to other humans (non-experts)

**Capabilities of Expert System**:
Can Do: 
- Advising
- Instructing and assisting human in decision making
- Demonstrating
- Deriving a solution
- Diagnosing
- Explaining
- Interpreting input
- Predicting Results
- Justifying the conclusion
- Suggesting alternative options to a problem
Cannot Do:
- Substituting human decision makers
- Possessing human capabilities
- Producing accurate output for inadequate knowledge base
- Refining their own knowledge

**Components of Expert System**:
* *Knowledge Base*: Contains the domain knowledge
* *Inference* (Reason(Thinking)): makes logical deductions based upon the knowledge in the knowledge base.
* *User Interface*: a facility for the user to interact with the Expert System.

![[Pasted image 20251005225829.png]]

**Knowledge Base**: contains the domain knowledge necessary for understanding, formulating, and solving problems

**Two Basic Knowledge Base Elements**: 
- *Factual Knowledge*: widely shared, typically found in textbooks or journals, and commonly agreed upon by those knowledgeable in the particular field.
- *Heuristic Knowledge*: the less strictly defined, relies more on empirical data, more judgmental knowledge of performance.

**Knowledge Representation**: deals with the formal modeling of expert knowledge in a computer program.

**Knowledge Representation must support**:
- Acquiring (new) knowledge
- Retrieving knowledge
- Reasoning with knowledge

**Knowledge Representation Schemas**:
- *Production Rules*: Expert systems that represent domain knowledge using production rules are called **rule-based expert systems**.
- *Frames*
- *Semantic Objects*

**Rules as Knowledge Representation Technique**:

A *Rule* is defined as an IF-THEN structure that relates given information or facts in the IF part to some action in the THEN part.

![[Pasted image 20251005232608.png]]
![[Pasted image 20251005232624.png]]

The *antecedent* of a rule incorporates two parts:
- Object (linguistic object)
- Value
The *Operator* identifies the object and assigns the value.
- *Operators* such as is, are, is not, are not, are used to assign a **symbolic value** to a linguistic object.
- *Mathematical Operators* can also be used to define an object as numerical and assign it to the numerical value.

**Main Players in Expert System Development Team**

**Domain Expert**: knowledgeable and skilled person capable of solving problems in a specific area or domain.

**Knowledge Engineer**: establishes what reasoning methods the expert uses to handle facts and rules and decides how to represent them in the expert system.

**Programmer**: the person responsible for the actual programming, describing the domain knowledge in terms that a computer can understand.

**Project Manager**: checks if all deliverables and milestones are met, interacts with the expert, knowledge engineer, programmer, and end-user.

**End-User**: the person who uses the expert uses.

**Structure of a Rule-Based Expert System**

**Knowledge Base**: contains the domain knowledge which are represented as a set of rules.
- If the condition part of a rule is satisfied, the rule is said to fire and the action part is executed.

**Database**: includes a set of facts used to match against the IF(condition) parts of rules stored in the knowledge base.

**Inference Engine**: links the rules given in the knowledge base with the facts provided in the database.

**Explanation Facilities**: enable the user to ask the expert system.

**User Interface**: the means of communication between a user seeking a solution to the problem and an expert system.

**Forward Chaining Technique**:

Forward Chaining is the **Data-Driven Reasoning**.
- The reasoning starts from the known data and proceeds forward with that data.
- Each time only the top most rule is executed (in *CLIPS* bottom most rule is executed first).
- When fired, the rule adds a new fact in the database
- Any rule can be executed only once
- The match-fire cycle stops when no further rules can be fired

**Backward Chaining Technique**:

Backward Chaining is the **Goal-Driven Reasoning**.

- An ES has the goal (a hypothetical solution) and the inference engine attempts to find the evidence to prove it.
- First, the knowledge base is searched to find rules that might have the desired solution.
- Such rules must have the goal in their THEN(action) parts
- If such rule is found and its IF(condition) part matches data in the database, then the rule is fired and the goal is proved.
- IF such rule is not found, the inference engine puts aside the rule it is working with (the rule is said to be stacked) and sets up a new goal (subgoal) to prove the IF part of this rule.
- Then the knowledge base is searched again for rules that can prove the subgoal.
- The inference engine repeats the process of stacking the rules until no rules are found in the knowledge base to prove the current subgoal.

**Comparison**
![[Pasted image 20251006001607.png]]
![[Pasted image 20251006001618.png]]

**How do we choose between FC and BC?

- **Forward Chaining**: If an expert first needs to gather some information and then tries to infer from it whatever can be inferred(no specific goal).
- **Backward Chaining**: If your experts begins with a hypothetical solution (goal) and then attempts to find facts to prove it.

**Conflict Resolution**
- Fire the rule with the highest priority
- Fire the most specific rule (longest matching strategy)
- Fire the rule that uses the data most recently entered in the database
- Fire the rule with the most preferable outcome based on weight

**Advantages of Rule-Based Expert System**
- Natural Knowledge Representation
- Uniform Structure
- Separation of Knowledge from its processing
- Dealing with incomplete and uncertain knowledge

**Disadvantages of Rule-Based Expert System**
- Opaque relations between rules
- Ineffective search strategy
- Inability to learn