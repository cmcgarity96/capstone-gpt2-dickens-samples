This folder contains samples from the GPT-2 model finetuned for 12K steps on the following 8 Dickens books:

-A Tale of Two Cities
-David Copperfield
-Great Expectations
-Little Dorrit
-Oliver Twist
-Our Mutual Friend
-The Old Curiousity Shop
-The Posthumous Papers of the Pickwick Club

We were able to finetune OpenAI's GPT-2 to produce text more in line with that of a Dickens novel by using the package gpt-2-simple, developed by Max Woolf to give researchers a way to easily finetune and work with GPT-2.  Max Woolf's work can be found on his GitHub, minimaxir.

Each text file contains ten samples, each with a different pretext, or input, for the model to start on.  Three of them were Dickens quotes, the citation was left out of the input.  Unlike standard GPT-2, the generate function for gpt-2-simple actually places the prefix, or input, at the top of every sample.  Keep this in mind when viewing the samples that the pretext is the first token at the top of each sample.

Additionally, GPT-2 is known to sometimes get stuck in a repetitive loop when it is outputting, or it will suddenly change subjects or lack coherency.  These issues are mentioned by the developers.  Some of these samples contain examples of this behaviour.

The four different inputs were as follows:

-CHAPTER 1

-'I see a beautiful city and a brilliant people rising from this abyss, and, in their struggles to be truly free, in their triumphs and defeats, through long long to come, I see the evil of this time and of the previous time of which this is the natural birth, gradually making expiation for itself and wearing out.’ -Dickens, A Tale of Two Cities

-'I am a disappointed drudge, sir. I care for no man on earth, and no man on earth cares for me. No man on earth has ever shown a light to me.’ -Dickens, A Tale of Two Cities

'Liberty, equality, fraternity, or death; - the last, much the easiest to bestow, O Guillotine!' -Dickens, A Tale of Two Cities


The CHAPTER 1 prefix was chosen to see what the model would generate without any input other than a chapter title.  The Dickens quotes were chosen randomly from an assortment of Dickens quotes, with no regard to which book they came from.  They are coincidentally all from the same book.  