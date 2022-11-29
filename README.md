```C
#include "me.h"

int main(void)
{
    env_t *world = init_world();
    entity_t me = {
        .name = strdup("Mathieu Barral"),
        .age = 20,
        .country = strdup("France"),
        .city = strdup("Montpellier"),
        .job = strdup("Student"),
        .school = strdup("Epitech"),
        .skills = {"C", "C++", "Asm", "Rust", "Java", "Python", "Haskell"},
        .interest = {
            "system",
            "low-level",
            "embedded",
            "cybersecurity",
            "devops"
        },
        .gpg_key_id = strdup("2EDD165AFD467745")
    };

    push_to_world(world, &me);
    free(world);
    return (0);
}
```
