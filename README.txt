Each folder contains 40 samples each from the GPT-2 355M model.  Four different inputs were used, and 10 samples were generated from each input.  

The folder gpt2reg_samples contains 10 samples each from the four chosen inputs generated on the pretrained GPT-2 model with NO finetuning, just the model as it is from OpenAI's GitHub.  

The folder dickens8_samples contains 10 samples each from the four chosen inputs, generated on the GPT-2 model finetuned on 12k steps with 8 Dickens books.  The specific books can be found under the README in that file.

The folder dickens15_samples contains 10 samples from each of the four chosen inputs, generated on the GPT-2 model finetuned on 12k steps with 15 Dickens books.  The specific books can be found under the README in that file.

The four different inputs were as follows:

-CHAPTER 1

-'I see a beautiful city and a brilliant people rising from this abyss, and, in their struggles to be truly free, in their triumphs and defeats, through long long to come, I see the evil of this time and of the previous time of which this is the natural birth, gradually making expiation for itself and wearing out.’ -Dickens, A Tale of Two Cities

-'I am a disappointed drudge, sir. I care for no man on earth, and no man on earth cares for me. No man on earth has ever shown a light to me.’ -Dickens, A Tale of Two Cities

'Liberty, equality, fraternity, or death; - the last, much the easiest to bestow, O Guillotine!' -Dickens, A Tale of Two Cities

The CHAPTER 1 prefix was chosen to see what the model would generate without any input other than a chapter title.  The Dickens quotes were chosen randomly from an assortment of Dickens quotes, with no regard to which book they came from.  They are coincidentally all from the same book.  

We were able to finetune OpenAI's GPT-2 to produce text more in line with that of a Dickens novel by using the package gpt-2-simple, developed by Max Woolf to give researchers a way to easily finetune and work with GPT-2.  Max Woolf's work can be found on his GitHub, minimaxir.