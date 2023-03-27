#include <iostream>
using namespace std;

class Automaton {
public:
  virtual void makefunction() {
    cout << "The is an automaton functioning" << endl;
  }
};

class DFA : public Automaton {
public:
  void makefunction() {
    cout << "This sequence is a Deterministic Finite Automata, extending the Automaton Class" << endl;
  }
};

class NFA : public Automaton {
public:
  void makeFunction() {
    cout << "This sequence is a Non-Deterministic Finite automata extending the Automaton Class" << endl;
  }
};

int main() {
	string sequence;
	cout<<"Enter a sequence:";
	cin>>sequence;
	
	char const* chrarry=sequence.c_str();
	int counter;
	for(int i=0;i<sizeof(chrarry)/sizeof(chrarry[0]);i++)
	{
		for(int j=i+1;j<sizeof(chrarry)/sizeof(chrarry[0]);j++)
		{
			if(chrarry[j]==chrarry[i])
			{
				counter++;
			}
		}
	}
	
	
  Automaton* func[2];
  DFA dfa;
  NFA nfa;

  func[0] = &dfa;
  func[1] = &nfa;

  if(counter>0){
  	func[0]->makefunction();
  }
  else{
  	func[1]->makefunction();
  }

  return 0;
}
