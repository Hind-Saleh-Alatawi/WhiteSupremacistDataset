# TwitterWhiteSupremacistDataset
A dataset for white supremacist tweets on twitter 
We had to collect the most recent white supremacist terms from a recently available platform such as Twitter. We select a randomly sample of 1,999 tweets and annotate the tweets in Amazon Mechanical Turk (AMT) ("Amazon Mechanical Turk," 2018). We then annotated the data, we chose the annotators to be from North America to ensure they have sufficient knowledge and culture, and they have at least 85% hit approval which is criteria for trusted annotators in AMT. 
The guidelines of the annotation are presented in Appendix A – Annotation Guidelines of White Supremacist Tweets. The annotation form initially consists of four labels as following:

•	Explicit White Supremacist: the user expresses his feelings with intended explicit white supremacist hate text either when they attack other races or claim that they are undermined by others.
e.g. “White Nationalism is simply the belief in homeland and self-determination for White people to describe that, and people who believe in it as “enemies of peace” is a complete disgrace.”

•	Implicit White Supremacist: when they express their hate intent indirectly, the sentence seems totally neutral because it does not include hate terms, but the intent from it is hate.
e.g. “We own our diversity, leave our country.”

•	Other Hate Speech: any hate text other than white supremacist hate text such as misogyny (woman hater), nationality, gender tendency hate speech.
e.g. “there are plenty women as stupid as you in this world dear, I’m sure he’ll be fine”

•	Neutral: when the sentence includes:
        • Neither positive nor negative text e.g. weather situation.
        • Positive (any normal text does not have an attack on others).
        • Unknown text (when you cannot decide it is positive or negative e.g. " to be against immigration does not mean to kill people" or because of the incomplete context     e.g."die for them").
        • The text includes hate terms with no hate intent (e.g. news with no hate intent).
        
 The Cohen kappa score of four labels Twitter dataset is 0.0706,so we collapse the four labels to binary labels (white supremacy or non-white supremacy) in which explicit and implicit white supremacy were collapsed into a ‘white supremacy’ label, and the ‘neutral’ and other hate categories were collapsed into ‘non-white supremacy’ because our goal was to detect white supremacists in particular. 
 
We calculated cohen’s kappa coefficient κ for the two labels (0 for not a white supremacist, 1 for white supremacist) of all annotators which does not exceed 0.11 Cohen’s kappa score. The disagreement is due to the difficulty in detecting implicit white supremacy hate speech as they understand different meanings based on the knowledge and history of white supremacists. Furthermore, Schmidt and Wiegand (2017) recognized from previous studies that the hate speech annotation process is reasonably ambiguous, which results in low agreement scores. To handle the annotators’ disagreements, we used a voting strategy by choosing the most common label among the three annotators, so if at least two annotators agreed on one label, either 0 or 1, this label will be used as the final tweet label. 
