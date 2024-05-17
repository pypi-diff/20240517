# Comparing `tmp/bhalaho-0.2.tar.gz` & `tmp/bhalaho-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhalaho-0.2.tar", last modified: Thu May 16 22:42:58 2024, max compression
+gzip compressed data, was "bhalaho-0.3.tar", last modified: Fri May 17 06:19:30 2024, max compression
```

## Comparing `bhalaho-0.2.tar` & `bhalaho-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 22:42:58.878158 bhalaho-0.2/
--rw-rw-rw-   0        0        0     1041 2024-05-16 22:19:08.000000 bhalaho-0.2/LICENSE
--rw-rw-rw-   0        0        0       72 2024-05-16 22:19:58.000000 bhalaho-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0       75 2024-05-16 22:42:58.871429 bhalaho-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-05-16 21:22:32.000000 bhalaho-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 22:42:58.839193 bhalaho-0.2/bhalaho/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:58:36.000000 bhalaho-0.2/bhalaho/__init__.py
--rw-rw-rw-   0        0        0    30234 2024-05-16 22:15:13.000000 bhalaho-0.2/bhalaho/daoa.py
--rw-rw-rw-   0        0        0      756 2024-05-16 21:25:52.000000 bhalaho-0.2/bhalaho/download.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:42:58.871429 bhalaho-0.2/bhalaho.egg-info/
--rw-rw-rw-   0        0        0       75 2024-05-16 22:42:58.000000 bhalaho-0.2/bhalaho.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-16 22:42:58.000000 bhalaho-0.2/bhalaho.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 22:42:58.000000 bhalaho-0.2/bhalaho.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 22:42:58.000000 bhalaho-0.2/bhalaho.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 22:42:58.878158 bhalaho-0.2/setup.cfg
--rw-rw-rw-   0        0        0      211 2024-05-16 22:42:53.000000 bhalaho-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:19:30.012427 bhalaho-0.3/
+-rw-rw-rw-   0        0        0     1041 2024-05-16 22:19:08.000000 bhalaho-0.3/LICENSE
+-rw-rw-rw-   0        0        0       72 2024-05-16 22:19:58.000000 bhalaho-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0       75 2024-05-17 06:19:30.008278 bhalaho-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-05-16 21:22:32.000000 bhalaho-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 06:19:29.956927 bhalaho-0.3/bhalaho/
+-rw-rw-rw-   0        0        0        0 2024-05-16 20:58:36.000000 bhalaho-0.3/bhalaho/__init__.py
+-rw-rw-rw-   0        0        0    30568 2024-05-17 06:18:28.000000 bhalaho-0.3/bhalaho/daoa.py
+-rw-rw-rw-   0        0        0      756 2024-05-16 21:25:52.000000 bhalaho-0.3/bhalaho/download.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:19:30.000187 bhalaho-0.3/bhalaho.egg-info/
+-rw-rw-rw-   0        0        0       75 2024-05-17 06:19:29.000000 bhalaho-0.3/bhalaho.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-17 06:19:29.000000 bhalaho-0.3/bhalaho.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 06:19:29.000000 bhalaho-0.3/bhalaho.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 06:19:29.000000 bhalaho-0.3/bhalaho.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 06:19:30.012427 bhalaho-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      211 2024-05-17 06:19:22.000000 bhalaho-0.3/setup.py
```

### Comparing `bhalaho-0.2/LICENSE` & `bhalaho-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bhalaho-0.2/bhalaho/daoa.py` & `bhalaho-0.3/bhalaho/daoa.py`

 * *Files 8% similar despite different names*

```diff
@@ -775,147 +775,105 @@
     printf("Minimum cost of the Hamiltonian Cycle: %d\n", tsp(graph, 1 << start, start, dp));
 
     return 0;
 }
 
 '''
 a15_puzzle = '''
-#include <stdio.h>
-#include <stdlib.h>
-#include <stdbool.h>
-#include <limits.h>
+#include<stdio.h>
+#include<stdlib.h>
 
 #define N 4
 
-// Structure to store the state of the puzzle
-typedef struct {
-    int puzzle[N][N]; // 4x4 puzzle grid
-    int x, y; // Coordinates of the empty space
-    int cost; // Cost of the current state
-} State;
-
-// Function to create a new State
-State* newState(int puzzle[N][N], int x, int y, int cost) {
-    State* state = (State*)malloc(sizeof(State));
-    if (state != NULL) {
-        for (int i = 0; i < N; i++) {
-            for (int j = 0; j < N; j++) {
-                state->puzzle[i][j] = puzzle[i][j];
-            }
-        }
-        state->x = x;
-        state->y = y;
-        state->cost = cost;
-    }
-    return state;
-}
-
-// Function to swap two tiles in the puzzle
-void swap(int* a, int* b) {
-    int temp = *a;
-    *a = *b;
-    *b = temp;
-}
-
-// Function to check if the puzzle is solved
-bool isSolved(int puzzle[N][N]) {
-    int count = 1;
-    for (int i = 0; i < N; i++) {
-        for (int j = 0; j < N; j++) {
-            if (puzzle[i][j] != count && !(i == N - 1 && j == N - 1))
-                return false;
-            count++;
-        }
-    }
-    return true;
-}
-
-// Function to calculate the Manhattan distance heuristic
-int manhattanDistance(int puzzle[N][N]) {
-    int distance = 0;
-    for (int i = 0; i < N; i++) {
-        for (int j = 0; j < N; j++) {
-            int value = puzzle[i][j];
-            if (value != 0) {
-                int targetX = (value - 1) / N;
-                int targetY = (value - 1) % N;
-                distance += abs(i - targetX) + abs(j - targetY);
+int getInvCount(int *arr){
+    int inv_count = 0;
+    for (int i = 0; i < N*N - 1; i++)
+    {
+        for (int j = i+1; j < N*N; j++)
+        {
+            if (arr[j] && arr[i] && arr[i] > arr[j])
+            {
+                inv_count++;
             }
+            
         }
+        
     }
-    return distance;
+    return inv_count;
 }
 
-// Function to check if a move is valid
-bool isValidMove(int x, int y) {
-    return (x >= 0 && x < N && y >= 0 && y < N);
+int findPosition( int puzzle[N][N]){
+    for (int i = N -1; i>= 0; i--)
+    {
+        for (int j = N - 1; j >= 0; j --)
+        {
+            if (puzzle[i][j] == 0)
+            {
+                return N - i;
+            }
+        }
+    }
 }
-
-// Function to perform a move in the puzzle
-State* move(State* state, int newX, int newY) {
-    if (!isValidMove(newX, newY))
-        return NULL;
-    State* newState = newState(state->puzzle, state->x, state->y, state->cost + 1);
-    swap(&(newState->puzzle[state->x][state->y]), &(newState->puzzle[newX][newY]));
-    newState->x = newX;
-    newState->y = newY;
-    return newState;
+int isSolvable(int puzzle[N][N]){
+    int invcount =  getInvCount((int *)puzzle);
+    if (N  & 1)
+        return !(invcount & 1);
+    else
+    {
+        int pos = findPosition(puzzle);
+        if (pos & 1)
+        {
+            return !(invcount & 1);
+        }
+        else
+        {
+            return invcount & 1;
+        }
+    }
 }
-
-// Function to find the minimum cost state
-State* minCostState(State* states[], int n) {
-    State* minState = states[0];
-    for (int i = 1; i < n; i++) {
-        if (states[i]->cost < minState->cost)
-            minState = states[i];
+int getManhattanDistance(int value,int row,int col){
+    if (value == 0)
+    {
+        return 0;
     }
-    return minState;
+    int goalRow = (value -1) / N;
+    int goalCol = (value - 1) % N;
+    return abs(row - goalRow) + abs(col - goalCol);
 }
 
-// Function to solve the Fifteen Puzzle using Branch and Bound
-void solveFifteenPuzzle(int initial[N][N]) {
-    int dx[] = {0, 0, 1, -1};
-    int dy[] = {1, -1, 0, 0};
-    int goal[N][N] = {
-        {1, 2, 3, 4},
-        {5, 6, 7, 8},
-        {9, 10, 11, 12},
-        {13, 14, 15, 0}
-    };
-    State* initialState = newState(initial, 3, 3, 0);
-    State* states[N*N*N*N];
-    int count = 0;
-    states[count++] = initialState;
-
-    while (true) {
-        State* currentState = minCostState(states, count);
-        if (isSolved(currentState->puzzle)) {
-            printf("Solution found with cost: %d\n", currentState->cost);
-            break;
-        }
-        for (int i = 0; i < 4; i++) {
-            int newX = currentState->x + dx[i];
-            int newY = currentState->y + dy[i];
-            State* newState = move(currentState, newX, newY);
-            if (newState != NULL) {
-                states[count++] = newState;
-            }
+int calculateTotalCost(int puzzle[N][N]){
+    int totalCost = 0;
+    totalCost += getInvCount((int *) puzzle);
+    for (int i = 0; i < N; i++)
+    {
+        for (int j = 0; j < N; j++)
+        {
+            totalCost += getManhattanDistance(puzzle[i][j],i,j);
         }
     }
+    return totalCost;
 }
 
-// Main function
-int main() {
-    int initial[N][N] = {
+int main()
+{
+    int puzzle[N][N] = {
         {1, 2, 3, 4},
-        {5, 6, 7, 8},
-        {9, 10, 0, 12},
-        {13, 14, 11, 15}
+        {5, 6, 0, 8},
+        {9, 10, 7, 11},
+        {13, 14, 15, 12},
     };
-    solveFifteenPuzzle(initial);
+
+    if (!isSolvable(puzzle))
+    {
+        printf("Not Solvable\n");
+        return 0;
+    }
+
+    int totalCost = calculateTotalCost(puzzle);
+    printf("Total Cost: %d\n", totalCost);
     return 0;
 }
 '''
 
 strassens_detail = '''
 #include <stdio.h>
 #include <stdlib.h>
@@ -1025,15 +983,15 @@
             printf("%d\t", matrix[i][j]);
         }
         printf("\n");
     }
 }
 
 int main() {
-    int n = 4; // Size of matrices
+     const int n = 4; // Size of matrices
     int A[n][n] = {{1, 2, 3, 4},
                    {5, 6, 7, 8},
                    {9, 10, 11, 12},
                    {13, 14, 15, 16}};
     int B[n][n] = {{17, 18, 19, 20},
                    {21, 22, 23, 24},
                    {25, 26, 27, 28},
@@ -1085,25 +1043,110 @@
 
     printf("Number of ways to make %d using the given coins: %d\n", amount, coinChange(coins, n, amount));
     
     return 0;
 }
 
 '''
+job_sequencing = '''
+// C program for the above approach
+ 
+#include <stdbool.h>
+#include <stdio.h>
+#include <stdlib.h>
+ 
+// A structure to represent a job
+typedef struct Job {
+   
+    char id; // Job Id
+    int dead; // Deadline of job
+    int profit; // Profit if job is over before or on
+                // deadline
+} Job;
+ 
+// This function is used for sorting all jobs according to
+// profit
+int compare(const void* a, const void* b)
+{
+    Job* temp1 = (Job*)a;
+    Job* temp2 = (Job*)b;
+    return (temp2->profit - temp1->profit);
+}
+ 
+// Find minimum between two numbers.
+int min(int num1, int num2)
+{
+    return (num1 > num2) ? num2 : num1;
+}
+ 
+// Returns maximum profit from jobs
+void printJobScheduling(Job arr[], int n)
+{
+    // Sort all jobs according to decreasing order of profit
+    qsort(arr, n, sizeof(Job), compare);
+ 
+    int result[n]; // To store result (Sequence of jobs)
+    bool slot[n]; // To keep track of free time slots
+ 
+    // Initialize all slots to be free
+    for (int i = 0; i < n; i++)
+        slot[i] = false;
+ 
+    // Iterate through all given jobs
+    for (int i = 0; i < n; i++) {
+       
+        // Find a free slot for this job (Note that we start
+        // from the last possible slot)
+        for (int j = min(n, arr[i].dead) - 1; j >= 0; j--) {
+           
+            // Free slot found
+            if (slot[j] == false) {
+                result[j] = i; // Add this job to result
+                slot[j] = true; // Make this slot occupied
+                break;
+            }
+        }
+    }
+ 
+    // Print the result
+    for (int i = 0; i < n; i++)
+        if (slot[i])
+            printf("%c ", arr[result[i]].id);
+}
+ 
+// Driver's code
+int main()
+{
+    Job arr[] = { { 'a', 2, 100 },
+                  { 'b', 1, 19 },
+                  { 'c', 2, 27 },
+                  { 'd', 1, 25 },
+                  { 'e', 3, 15 } };
+    int n = sizeof(arr) / sizeof(arr[0]);
+    printf(
+        "Following is maximum profit sequence of jobs \n");
+ 
+    // Function call
+    printJobScheduling(arr, n);
+    return 0;
+}
+
+'''
+
 time_complexity = '''
 abhi baki hai daalna bhai , sabar rakho
 '''
 
 daoaexp = {
     'Prims.c' : prims,
     'Kruskal.c' : kruskal,
     'Dijkstra.c' : dijkstra,
     'Matrix Chain Multiplication.c' : matrix_chain_multiplication,
     'Longest_Common_Subsequence.c' : longest_common_subsequence,
-    '0/1 Knapsackdp.c' : knapsack,
+    'job_sequencing.c' : job_sequencing,
     'Fractional greedy Knapsack.c' : fractional_knapsack,
     'N-Queens.c' : n_queens,
     'Sum_of_Subset.c' : sum_of_subset,
     'KMP.c' : kmp,
     'Coin Change Greedy.c' : coin_change_greedy,
     'TSP_dp.c' : TSP_dp,
     '15 Puzzle.c' : a15_puzzle,
```

### Comparing `bhalaho-0.2/bhalaho/download.py` & `bhalaho-0.3/bhalaho/download.py`

 * *Files identical despite different names*

