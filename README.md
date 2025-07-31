# Longest-Common-Prefix

public String longestCommonPrefix(String[] strs) {

        // I used "result" variable to store "longest Common Prefix"
         StringBuilder result = new StringBuilder();

    // Sort the array
    Arrays.sort(strs);

    // Get the first and last strings
    char[] first = strs[0].toCharArray();
    char[] last = strs[strs.length - 1].toCharArray();

    // Start comparing
    for (int i = 0; i < first.length; i++) {
      if (first[i] != last[i])
        break;
      result.append(first[i]);
    }

    return result.toString();
        
    }
