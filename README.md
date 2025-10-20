# CodeWars-Sum-of-array-singles-7-kyu---Passed-
In this Kata, you will be given an array of numbers in which two numbers occur once and the rest occur only twice. Your task will be to return the sum of the numbers that occur only once.  For example, repeats([4,5,7,5,4,8]) = 15 because only the numbers 7 and 8 occur once, and their sum is 15. Every other number occurs twice.


In this Kata, you will be given an array of numbers in which two numbers occur once and the rest occur only twice. Your task will be to return the sum of the numbers that occur only once.

For example, repeats([4,5,7,5,4,8]) = 15 because only the numbers 7 and 8 occur once, and their sum is 15. Every other number occurs twice.

#[cfg(test)]
mod tests {
    use super::repeats;

    #[test]
    fn basic_tests() {
        assert_eq!(repeats(&vec![4, 5, 7, 5, 4, 8]), 15);
        assert_eq!(repeats(&vec![9, 10, 19, 13, 19, 13]), 19);
        assert_eq!(repeats(&vec![16, 0, 11, 4, 8, 16, 0, 11]), 12);
        assert_eq!(repeats(&vec![5, 17, 18, 11, 13, 18, 11, 13]), 22);
        assert_eq!(repeats(&vec![5, 10, 19, 13, 10, 13]), 24);
    }
}
