---
layout: function
short_name: KKKK
qualified_name: nda::KKKK
description_brief: One line description of the function
description: |
    Here comes the long description of the nice function
params_description:
  i: Documentation of i
  # YAML::Newline + Comment
  #  Cf doc : yaml cpp know map, vector + << : recursive

  a_long_param_name: |
    Documentation of j which can be reaally **really** long
    
    even with formulas $a = \pi$ inline or not
    
    $$ \int f(x) dx = \dfrac{\pi}{2}$$
    
    This is true for any field which we can document in YAML.
    
    Even with code
    ```cpp
        int main() {
          a = f.method(x);
        }
    ```

return: What does it return
includer: nda.hpp

overload_description:  # Edit here the overload short description
  int nda::KKKK(int i): This takes only one variable !
  int nda::KKKK(int i, int j): __MISSING__
  int nda::KKKK(double x, int j): Who designed this API ?

example: # For several example, put examples and make a list
  compile: true  # Or
  code: |
    #include <vector>
    int main() {
      int i=3;
        auto g = gf<imfreq>{beta,3, shape};
    };

see-also:
  nda::bad: bad is indeed an excellent functoin # TOOL : Automatically find the desc_brief and complete the namesapce ?
  nda::K3:

overloads:  # DO NOT EDIT BELOW THIS LINE
  int nda::KKKK(int i):
    namespaces: [nda]
    rtype: int
    params:
      - type: int
        link: KKKK
        name: i
    definition_location: cls1.cpp
  int nda::KKKK(int i, int j):
    namespaces: [nda]
    rtype: int
    params:
      - type: int
        link: KKKK
        name: i
      - type: int
        name: j
  int nda::KKKK(double x, int j):
    namespaces: [nda]
    rtype: int
    params:
      - type: double
        name: x
      - type: int
        name: j
    definition_location: /Users/oparcollet/B/cpp2pyv2/cls1.cpp:20:3
    
  int nda::KKKK(double x, int j):
    namespaces: [nda]
    rtype: int
    params:
      - type: double
        name: x
      - type: std::vector<gf<imfreq, matrix_valued>>
        name: j
      - type: std::vector<gf<imfreq, matrix_valued>>
        name: j
      - type: std::vector<gf<imfreq, matrix_valued>>
        name: j
      - type: std::vector<gf<imfreq, matrix_valued>>
        name: j
      - type: std::vector<gf<imfreq, matrix_valued>>
        name: j
    definition_location: /Users/oparcollet/B/cpp2pyv2/cls1.cpp:20:3

...

I can put something here as well....



