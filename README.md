#include <iostream>
#include <vector>
using namespace std;

void show(vector<double> v) {
	for (int i = 0; i < v.size(); i++) {
		cout << v[i] << ' ';
		
	}cout << endl;
}

int main() {
	vector<double> v = { 1,2,3,5,8 };
	/*show(v);
	//v.resize(3);
	//v.push_back(12);
	show(v);
	//v.pop_back();
	show(v);
	cout << v.capacity() << endl;*/ //capacity-колво элементов в массиве size-колво видимых эл
	v.reserve(80);
	for (int i = 0; i < 100; i++) {
		v.push_back(i);
		cout << v.size() << ' ' << v.capacity() << endl;
	}
}
