# Search Engine

This project is a simple search engine application that reads text files, builds a Binary Search Tree (BST) of words, and supports searching and traversing the BST. The GUI is built using Java Swing.

## Features

1. **File Selection:** Select multiple text files to read and process.
   
2. **Ignore List:** Specify a file containing words to be ignored during processing.
   
3. **Binary Search Tree:** Insert words into a BST, where each node contains a linked list of files where the word appears and the frequency of the word in each file.
   
4. **Search:** Search for a word in the BST and display the files and frequencies.
   
5. **Traversal:** Display the BST in InOrder, PreOrder, or PostOrder traversal.
    
6. **GUI:** User-friendly graphical interface for easy interaction.

## How to Use

1. **Prerequisites**

  - Java Development Kit (JDK) 8 or higher
  - A Java IDE or text editor
  - Swing library (usually included in the JDK)

2. **Running the Application**

  - Clone this repository to your local machine.
  - Open the project in your preferred Java IDE.
  - Compile and run the SearchEngine class.

## User Interface
**Buttons and Fields**

- **Select File:** Opens a file chooser to select text files for processing.
  
- **Select Ignore File:** Opens a file chooser to select a file containing words to be ignored.
  
- **Search:** Searches for the entered word in the BST and displays the results.
  
- **Order:** Displays the BST in the selected traversal order (InOrder, PreOrder, or PostOrder).
  
- **Text Fields:**
    - **´txt_searched:´** Enter the word to search.
    - **´txtArea_wordList:´** Displays the search results.
    - **´txtArea_bstOrder:´** Displays the traversal results.

## Functionality

1. **File Selection:**

    - Click the "Select File" button to choose multiple text files. The selected files are processed, and words are inserted into the BST.
    - Click the "Select Ignore File" button to choose a file containing words to ignore during processing.

2. **BST Insertion:**
    - Words from the selected files are inserted into the BST.
    - Each node in the BST contains a linked list of files and the frequency of the word in each file.

3. **Searching:**

    - Enter a word in the txt_searched field and click the "Search" button.
    - The search results, including the files and frequencies, are displayed in txtArea_wordList.

4. **Traversal:**

    - Select a traversal order (InOrder, PreOrder, or PostOrder) from the comboBox_order and click the "Order" button.
    - The traversal results are displayed in txtArea_bstOrder.

## Code Structure

**Packages**
  - **SearchEngine:** Contains all the classes for the application.

**Classes**
1. **BinarySearchTree:** Implements the BST with nodes containing words, file lists, and frequencies.

2. **BSTNode:** Represents a node in the BST.
   
3. **LinkedList:** Represents a linked list of files for each word in the BST.
   
4. **LinkedListNode:** Represents a node in the linked list.
   
5. **SearchEngine:** Implements the GUI and handles file selection, word processing, and user interactions.

**Methods**

- BinarySearchTree:
  
    - **´insert()´**: Inserts a word into the BST.
    - **´inorder()´**, **´preorder()´**, **´postorder()´**: Traverses the BST.
    - **´printWordsCount()´**: Searches for a word and prints the file list and frequencies.

- LinkedList:

    - **´addFirst()´**: Adds a file to the linked list.
    - **´getLinkedListString()´**: Returns a string representation of the linked list.

- SearchEngine:

    - **´btn_selectActionPerformed()´**, **´btn_ignoreListActionPerformed()´**, **´btn_orderActionPerformed()´**, **´btn_searchActionPerformed()´**: Handle button actions.
    - **´readWords()´**, **´chooseFiles()´**: Handle file reading and processing.

## Acknowledgments
- Inspired by simple search engine algorithms and BST implementations.

For any questions or issues, please open an issue on GitHub.
 
## Screenshots

![Resim1](https://github.com/ekrem-bas/SearchEngine/assets/145195096/7bfaf7ae-b2be-413f-b063-1229ec068a8e)

![Resim2](https://github.com/ekrem-bas/SearchEngine/assets/145195096/3ea55cf3-de6a-4d22-99c7-e96b315386c9)

![Resim3](https://github.com/ekrem-bas/SearchEngine/assets/145195096/d8cdbf74-097a-47a6-b369-f813dae9fd4a)

![Resim4](https://github.com/ekrem-bas/SearchEngine/assets/145195096/1fc2da86-69e6-4134-bfa3-0bf91793af56)

![Resim5](https://github.com/ekrem-bas/SearchEngine/assets/145195096/8b490d1e-6785-4261-94d6-b61003421454)

![Resim6](https://github.com/ekrem-bas/SearchEngine/assets/145195096/5f60fd7f-cf52-4e26-b7f1-0561511efd01)
