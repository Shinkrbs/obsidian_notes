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
- Each time only the top most rule is executed