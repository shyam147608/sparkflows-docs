RemoveUnwantedCharacters
=========== 

This node removes unwanted characters

Input
--------------
It accepts a DataFrame as input from the previous Node

Type
--------- 

transform

Class
--------- 

fire.nodes.etl.NodeRemoveUnwantedCharacters

Fields
--------- 

.. list-table::
      :widths: 10 5 10
      :header-rows: 1

      * - Name
        - Title
        - Description
      * - inputCols
        - Input Columns
        - input columns
      * - removeWhitespaces
        - Remove Whitespaces
        - removes white space
      * - removeLetters
        - Remove Letters
        - removes letters
      * - removeDigits
        - Remove Digits
        - removes digits
      * - removeSigns
        - Remove Signs
        - removes signs
      * - removeCommas
        - Remove Commas
        - removes commas

Examples
----------

Input
----------

.. list-table:: 
   :widths: 10 10 30
   :header-rows: 1

   * - id
     - prodId
     - message
   
   * - 1.0
     - 0.0
     - this is not a 2 spam
     
   * - 2.0
     - 1.0
     - i am, going to work

   * - 3.0
     - 2.0
     - this is a spam
     
     
Parameters
-------------

.. list-table:: 
   :widths: 10 25
   :header-rows: 1
   
   * - Name
     - Value
     
   * - Input Columns
     - message
   
   * - Remove Whitespaces
     - true
   
   * - Remove Letters
     - false
     
   * - Remove Digits
     - true
     
   * - Remove Signs
     - true   
 
   * - Remove Commas
     - true
     
Output
----------

.. list-table:: 
   :widths: 10 10 30
   :header-rows: 1

   * - id
     - prodId
     - message
   
   * - 1.0
     - 0.0
     - thisisnotaspam
     
   * - 2.0
     - 1.0
     - iamgoingtowork

   * - 3.0
     - 2.0
     - thisisaspam   
