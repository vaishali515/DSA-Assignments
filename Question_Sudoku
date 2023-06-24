#include <bits/stdc++.h>
using namespace std;

// Knight Tour
// Generate All Binaries
#define Size 9
bool isEmpty(vector<vector<int>> &sudoku,int &row, int &col) {
      for (row = 0; row< Size; row++) {
          for (col= 0; col < Size; col++) {
              if (sudoku[row][col] ==0) {
                   return true;

              }
         }
    }
    return false;
}
 bool usedInRow(vector<vector<int>> &sudoku, const int row,int fill){
for(int j = 0;j<size;j++)
if(sudoku[row][j] == fill){
return true;
}
}
}

bool usedInRow(vector<vector<int>> &sudoku,const int col,int fill){
for(int j = 0;j<size;j++)
if(sudoku[i]col] == fill){
return true;
}
}
return false;
}

bool usedInBox(vector<vector<int>> &sudoku,const int row ,const int fill) {
row = row - row % 3;
col = col - col %3;
for(int i = 0;i<3;i++){
for(int j = 0;j<3;j++){
if(sudoku[i+row][j+col] == fill){
return true;
}
}
}
return false;

}

bool isSafe(vector<vector<int>> &sudoku,const int row,const int col,int fill){

return(!usedinRow(sudoku,row,col,fill)&& !usedIncol(sudoku,row,col,fill) &&!usedInBox(sudoku,row,col,fill)
}

bool solveSudoku(vector<vector<int>> &sudoku) {
     int row, col;
    for (row = 0;row < Size; row++){
        for(col = 0; col < Size; col++){
           if(sudoku[row][col]==0){
              found = true;
              break;
            }
       }
       if(found){
          break;
        }
       if(!found)   {
          return true
}
for(int i = 1; i<=9; i++){
    if(isSafe(sudoku, row, col, i)){
        sudoku[row][col]=i;
        if(solveSudoku(sudoku)){
              return true;
         }
         //backtracking
         sudoku[row][col]=0;
         }
     }
}
