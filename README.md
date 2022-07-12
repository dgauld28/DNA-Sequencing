# DNA-Sequencing
// Project : DNA Sequencing.
// Description : Determines whether there is a protein in a strand of DNA
// Author : Damian Gauld

public class DNA {
 
  public static void main(String[] args) {
 
    //  -. .-.   .-. .-.   .
    //    \   \ /   \   \ / 
    //   / \   \   / \   \  
    //  ~   `-~ `-`   `-~ `-

    // The three DNA strands

    String dna1 = "ATGCGATACGCTTGA";
    String dna2 = "ATGCGATACGTGA";
    String dna3 = "ATTAATATGTACTGA";

    // Test with dna1 below
    String dna = dna1;
    //System.out.println(dna.length());

    //Finding the Start & Stop Codon
    int index = dna3.indexOf("ATG");

    int index2 = dna3.indexOf("TGA");

    if(index != -1 && index2 != -1 &&(index2 - index) % 3 == 0) {
      System.out.println("All conditions are cleared.");

    }
    else {
      System.out.println("No protein.");
    }
 
  }
 
}
