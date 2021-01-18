  
package dayone

import java.io.File

fun main() {
    val input = File("src/main/kotlin/dayone/input")
        .readLines()
        .map { it.toInt() }

    fun solvePartOne(): Int = input
        .mapNotNull { a -> if (input.contains(2020 - a)) a * (2020 - a) else null }
        .first()

    fun solvePartTwo(): Int {
        for (a in input) {
            for (b in input) {
                for (c in input)
                    if (a + b + c == 2020) return a * b * c
            }
        }
        return 0
    }

    println(solvePartOne())
    println(solvePartTwo())
}
