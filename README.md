# openpet
Everything related to OpenMined and PET
Privacy-transparency tradeoff
Privacy is appropriate flow of information
Loss of Privacy is when this flow of information is 'uncontrolled'

## Information flow
- Challenges - leaky info flow, insufficient info flow
- Clarity on Contextual integrity
- Privacy dilemma vs transparency dilemma

## Privacy-transparency  tradeoff
- Traditional 
<img src="https://deeplearning.berlin/images/images/articles/2021-01-05-openmined-pt1/privacy-transparency-pareto-tradeoff.png" alt="Traditional" width="300"/>

- With Parento frontier 
<img src="https://deeplearning.berlin/images/images/articles/2021-01-05-openmined-pt1/moving-the-privacy-transparency-pareto-tradeoff.png" alt="With Parento frontier" width="300"/>

As shown above for the same amount of 'B' there is more 'A' (when compared to the 'Traditional'). Thus prviacy-transparency tradeoff - need not be a Zero sum game. Creating information flows within society that create social good.

## 3 technical problems
when addressed will take privacy-transaparency tradeoff in traditional realm to the realm of the pareto frontier

|Problem|definition|example|how to overcome?|
| --- | --- |--- | --- |
|Copy Problem|lose control over 'own' data once that data is shared, Difficultt to enforce |Digital Piracy| HIPPA or GDPR or CCPA DRM|
|Bundling problem | revealing unnecessary  / dditional information along with intended information | DL being verified for age, leaks address, AI Governance, Using CC for trial| --- |
|Recurisve enorcement problem | when enforcing privacy regulations who enfores the enforcer, data governance |--- | systems of decentralized governance |

## Structured Transparency
- enable transparency without the risk of misuse
- structured approach to analyze privacy issues
- Components of Structured Transparency


|Name|definition |how to overcome? techniques|
| --- | --- | --- |
|Input privacy|guarantee that one or more people can participate in a computation, in such a way that neither party learns anything about the other party’s inputs to the computation guarantee only protects the inputs to an information flow - concerned with the copy problem| PKI, HE, SMPC Additive Secret Sharing, shared governance,secured computation
|Output privacy| ensuring that certain subsets of information do not make it through the information flow. a degree of protection.  concerned with the bundling problem | Differential Privacy gives hard guarantee to output privacy, HE does not give a true guarantee of output privacy, Epsilon ɛ -privacy budget | 
|Input verification|Internal consistency   Threat from MTM | Tools include Digital Signatures, Certificates, CA, ZKP, Group Keys |  
|Output verification|verify that the outputs from a hidden information flow contain the relevant properties |  Explainability, Audit an algorithm, Remove bias |  
|Flow governance|change the guarantees in an information flow|unilateral governance - using PKI Consensu governance - Additive secret Sharing (SMPC)  |   


|function|components|
| --- | --- |
|guarantees about the inputs of an information flow| Input Privacy, Input verification|
|guarantees about the outputs of an information flow| Output Privacy, Output verification|
|relates to information that needs to be hidden|Input and output privacy|
| who is allowed to change the flow, as in change i/o privacy and verficiation guarantees|Flow governance|

