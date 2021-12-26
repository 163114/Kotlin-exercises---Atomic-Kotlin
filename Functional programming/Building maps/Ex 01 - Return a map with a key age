data class Person(
    val name: String,
    val age: Int
)

fun demographic(people: List<Person>): Map<Int, List<String>> {
    return people.groupBy(Person::age).mapValues {(_, group) ->
        group.map(Person::name)
    }
}

fun main(){
    val dataForPerson = listOf(
        Person("John", 22),
        Person("Johnny", 22),
        Person("Julia", 42))
    println(demographic(dataForPerson))
}
