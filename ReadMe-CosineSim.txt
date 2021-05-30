1. The notebook "CosineSim-Submit-OneBlock.ipynb" implements TruncatedSVD via sklearn.decomposition module   
2. We create a latent space consisting of 20 features.  There are 53424 users and 10000 books in the .csv files.  Clearly 20 may be too small
3. When you run the notebook, all the code executes to the 'end' (so the notebook isn't divided into 'blocks').  Once you run it, it loads the .csv files, creates the model, fits the model, and then asks you which of 3 options you want to do
4.  The 3 options are:
    1. Enter '1' to enter a book index and get similar books to it"
    2. Enter '2' to get a list of books between two indices"
    3. Enter '3' to see if a book is in the list"

5. Notes on OPTION '1'
You must already know what book index you want (the valid book indices are 1 thru 2099).  If you enter say '341' for book title 'Contact' you will see the following output (it'll show you the first 10 books that have a cosine similarity of 0.8 or above; it'll also give you the option to see all the books that have a cos-sim of 0.8 or above):

Books that are similar to 'Contact' follows:

2001: A Space Odyssey (Space Odyssey, #1)
A Brief History of Time
A Canticle for Leibowitz
Band of Brothers: E Company, 506th Regiment, 101st Airborne from Normandy to Hitler's Eagle's Nest
Childhood's End
Congo
Cosmos
Do Androids Dream of Electric Sheep?
Dune (Dune Chronicles #1)
Foundation (Foundation #1)

See all the books that are similar ('y' or 'n'): y


Foundation and Empire (Foundation #2)
I, Robot (Robot #0.1)
Jurassic Park (Jurassic Park, #1)
Neuromancer
Next
Prey
Red Mars (Mars Trilogy, #1)
Red Storm Rising
.
.
.

6. Notes on OPTION '2'
If you enter option 2, you will be asked for the "lower-bound index" and the "high-bound index" (i.e. the books which have an index in between these two values):
In the example below, I want to see which books have an index between 1000 and 1020

enter lower-bound index (between '1' and '2099'): 1000

enter high-bound index(between '1' and '{num_books_in_list-1}'): 1020

The output will show the index and the book associated with that index, as seen in the below output:

Index 1000, Title = 'Outlander (Outlander, #1)'

Index 1001, Title = 'Outliers: The Story of Success'

Index 1002, Title = 'P.S. I Love You'

Index 1003, Title = 'Pandemonium (Delirium, #2)'

Index 1004, Title = 'Paper Towns'

Index 1005, Title = 'Paradise Lost'

Index 1006, Title = 'Passion (Fallen, #3)'

Index 1007, Title = 'Patriot Games (Jack Ryan Universe, #2)'

Index 1008, Title = 'Pawn of Prophecy (The Belgariad, #1)'

Index 1009, Title = 'Peace Like a River'

Index 1010, Title = 'People of the Book'

Index 1011, Title = 'Perdido Street Station (Bas-Lag, #1)'

Index 1012, Title = 'Perfect Chemistry (Perfect Chemistry, #1)'

Index 1013, Title = 'Perfect Match'

Index 1014, Title = 'Perfume: The Story of a Murderer'

Index 1015, Title = 'Persepolis: The Story of a Childhood (Persepolis, #1)'

Index 1016, Title = 'Persuader (Jack Reacher, #7)'

Index 1017, Title = 'Persuasion'

Index 1018, Title = 'Pet Sematary'

Index 1019, Title = 'Peter Pan'



7. Notes on OPTION '3'
This option is to let you "browse" the database and look for book titles that you are interested in.  Suppose you want to find all books with the word 'Perfect' in it.  Use option 3, and enter 'Perfect', as seen below:

Enter book title to search for: Perfect

The first 7 characters, 'Perfect', is in the book list, 'Perfect Chemistry (Perfect Chemistry, #1)' has index 1012

The first 7 characters, 'Perfect', is in the book list, 'Perfect Match' has index 1013

The first 7 characters, 'Perfect', is in the book list, 'Picture Perfect' has index 1022

The first 7 characters, 'Perfect', is in the book list, 'The Perfect Storm: A True Story of Men Against the Sea' has index 1711