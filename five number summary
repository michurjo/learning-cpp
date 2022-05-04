#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;

int main() {
  int numberOfValues, middle;
  double datapoint, median, total, mean;
  vector <double> dataset;
  
  cout << "How many data values are in your set? ";
  cin >> numberOfValues;

  for(int i = 0; i < numberOfValues; i++){
    cout << "Enter a value: ";
    cin >> datapoint;
    dataset.push_back(datapoint);
    total = total + datapoint;
  }

  mean = total/numberOfValues;

  sort(dataset.begin(),dataset.end());

  for(int i = 0; i < numberOfValues; i++){
    cout << dataset[i] << "\n";  
  }
  system("clear");

  cout << "The minimum value is " << dataset[0] << "\n";
  cout << "The maximum value is " << dataset[dataset.size()-1] << "\n";

  if(numberOfValues % 2 == 1){
    cout << "The median is " << dataset[numberOfValues/2] << "\n";
  }
  else{
    middle = numberOfValues/2;
    median = (dataset[middle] + dataset[middle - 1])/2;
    cout << "The median is " << median << "\n";
  }

  cout << "The mean is " << mean << "\n";
  
  int number = dataset[0];
  int mode = number;
  int count = 1;
  int countMode = 1;
  int size = 5;
  for (int i=1; i<size; i++)
  {
    if (dataset[i] == number) 
    { // count occurrences of the current number
       ++count;
    }
    else
    { // now this is a different number
  
         count = 1; // reset count for the new number
         number = dataset[i];
    }
    if (count > countMode) {
                countMode = count;
                mode = number;
    }
  }
  
  cout << "The mode is " << mode << endl;
  
}
