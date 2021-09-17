# This will convert all strings to snake_case

def refactor_names(old_names: list):
    new_names = []
    for name in old_names:
        if name.isupper():
            name = name.lower()
        name = ''.join(f"_{letter.lower()}" if letter.isupper() else letter for letter in name)
        name = name.replace("__", "_")
        if name.startswith("_"):
            name = name.replace("_", "", 1)
        new_names.append(name)
    return new_names


if __name__ == '__main__':
    names = [
        "testeId", "Start_with_uppercase", "end_with_uppercasE", "middleUppercasse", "twoUpperCases",
        "underline_With_Uppercase", "ONLYUPPERCASE"]
    print(names)
    names = refactor_names(names)
    print(names)
