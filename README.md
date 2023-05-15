# Sunafu
Part1
#include <iostream>
#include <vector>
#include <string>

using namespace std;

int main() {
    int numDays;
    cout << "Enter number of days in the schedule: ";
    cin >> numDays;

    vector<string> schedule(numDays);
    for (int i = 0; i < numDays; i++) {
        cout << "Enter watering schedule for day " << i+1 << ": ";
        cin >> schedule[i];
    }

    cout << "\nWatering schedule:\n";
    for (int i = 0; i < numDays; i++) {
        cout << "Day " << i+1 << ": " << schedule[i] << endl;
    }

    return 0;
}
