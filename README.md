
![visitors](https://visitor-badge.laobi.icu/badge?page_id=COD3M4ST3R&left_color=black&right_color=transparent)



```cpp
class Me : public Human // weird mulfunctions keeps getting bigger and bigger, needs a fix a.s.a.p.
{
    protected:
        std::string m_address; // much protected.

    private:
        std::string m_name;
        std::string m_website; // you should check it is beautiful, expecially the parallax.
        std::string m_title;
        std::vector<std::string> m_fields;
        std::vector<std::string> m_languages;
        std::vector<std::string> m_technologies;

    public:
        static inline const std::string_view message = "Greetings, I hope you have an awesome day!";
        explicit Me(
            const std::string& p_gender, // it is a boolean. Just identifies itself as a string.
            const std::string& p_address, 
            const std::string& p_name,
            const std::string& p_website, 
            const std::string& p_title, 
            const std::vector<std::string>& p_fields, 
            const std::vector<std::string>& p_technologies,
            const std::vector<std::string>& p_languages = {"English", "German", "Turkish", "Gibberish"}
        ) : 
            Human((p_gender)),
            m_address(p_address), 
            m_name(p_name),
            m_website(p_website),
            m_title(p_title), 
            m_fields(p_fields), 
            m_technologies(p_technologies),
            m_languages(p_languages){}

        Me(Me&& other) noexcept :
            Human(std::move(other.get_gender())),
            m_address(std::move(other.m_address)),
            m_name(std::move(other.m_name)),
            m_website(std::move(other.m_website)),
            m_title(std::move(other.m_title)),
            m_fields(std::move(other.m_fields)),
            m_technologies(std::move(other.m_technologies)),
            m_languages(std::move(other.m_languages)) {}
};


int main(int argc, char *argv[])
{
    std::unique_ptr<Me> me = std::make_unique<Me>(
        "Male",
        "Frankfurt, GERMANY", 
        "Nadir Suhan ILTER",
        "suhan.website", 
        "Computer Engineer", 
        std::vector<std::string>{"Deep Learning", "Rockets", "Back-End", "Algorithms"}, 
        std::vector<std::string>{"Everything, just understand that people can learn; when they know what they need to learn."},
        std::vector<std::string>{"C", "C++", "C#", "Java", "Python", "BashScript", "R"}
    );
    
    return 0; // no worries, no problems.
}
```
