```C
#include "me.h"

int main(void)
{
    world_t *world = init_world();
    entity_t me = {
        .name = "Mathieu Barral",
        .age = 20,
        .country = "France",
        .city = "Montpellier",
        .job = "Student",
        .school = "Epitech",
        .skills = {"C", "C++", "Asm", "Go", "Zig", "Rust", "Python"},
        .interest = {
            "system",
            "low-level",
            "embedded",
            "cybersecurity",
            "devops"
        },
        .gpg_key_id = "2EDD165AFD467745"
    };

    push_to_world(world, &me);
    free(world);
    return (0);
}
```