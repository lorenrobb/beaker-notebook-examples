###.pdb to Chord Diagram/Conservation Graph

## Important notes:

* Make sure you have Biopython correctly installed (**pip install biopython**)

* Make sure you have an installed **tcoffee** module to generate the conservation scores (see **http://www.tcoffee.org/Projects/tcoffee/**)

* f your protein has more than 999 amino acids, edit the **aminoCount** variable, changing the sizes from 1000 to however big you need it to

* Make sure there are no extra lines in your .txt file

* Distances are measured from alpha carbon to alpha carbon (you can change this by editing line 68 and 74 to whichever atom you'd like to       measure to and from)

* Fasta files cannot contain "+" in their name. Please replace with some other character.

## Instructions:
* Put the following files in **~/.beaker/v1/web/pdbData** folder:

     -An empty file called matrix1.json
     
     -An empty file called teams.csv
     
     -An empty file called aligned.aln
     
     -An empty file called entropyScores.txt
     
     -An empty file called temp.aln
     
     -An empty file called temp.fast
     
     -style.css (available in text form below)
     
     -The .pdb file you want to read from
     
     -The .fasta file you want to read from (skim and remove bad sequences for best results)
     

* Change the **pdbFileName** and **fastaFileName** variables

* Change the  **upperLimit** and  **lowerLimit** variables (range in angstroms of distances between amino acids that you want to map on the chord diagram)

* Change **displayType** variable to display either temperature factor or conservation score on the outer ring

* Mouse over amino acids to isolate their chords, click "Get chord chart" to see all chords again

* Conservation scores are turned into a bar graph surrounding the chord diagram

* Table under diagram shows connections and distances from whichever AA you're mousing over