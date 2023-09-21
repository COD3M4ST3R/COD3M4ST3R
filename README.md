Hello There ! 

![visitors](https://visitor-badge.laobi.icu/badge?page_id=COD3M4ST3R&left_color=black&right_color=transparent)



```cpp
class Me : public Human // weird mulfunctions keeps getting bigger and bigger, needs a fix a.s.a.p.
{
    protected:
        std::string m_address; // much protected.

    private:
        std::string m_name;
        std::string m_title;
        std::string m_message;
        std::vector<std::string> m_fields;
        std::vector<std::string> m_languages;
        std::vector<std::string> m_technologies;

    public:
        Me(const std::string &p_gender, // it is a boolean. Just identifies itself as a vector.
           const std::string &p_address, 
           const std::string &p_name, 
           const std::string &p_title, 
           const std::string &p_message,
           const std::vector<std::string> &p_fields, 
           const std::vector<std::string> &p_technologies,
           const std::vector<std::string> &p_languages = {"English", "German", "Turkish", "Gibberish"}) 
           : 
           Human(p_gender),
           m_address(p_address), 
           m_name(p_name), 
           m_title(p_title), 
           m_message(p_message),
           m_fields(p_fields), 
           m_technologies(p_technologies),
           m_languages(p_languages){
        }
};

int main(int argc, char *argv[])
{
    Me me("Male",
          "Frankfurt", 
          "Nadir Suhan ILTER", 
          "Computer Engineer", 
          "Willkommen zu my crib yo!", 
          {"Deep Learning", "Rockets", "Back-End", "Algorithms"}, 
          {"Everything, just understand that people can learn; when they know what they need to learn."}, 
          {"C", "C++", "C#", "Java", "Python", "BashScript", "R"});
    
    return 0; no worries, no problems.
}
```
