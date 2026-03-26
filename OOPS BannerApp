import java.util.HashMap;

public class OOPSBannerApp {

  public static HashMap<Character, String[]> createCharacterMap() {
    HashMap<Character, String[]> charMaps = new HashMap<>();

    String[] OPattern = {
        "   ***   ",
        " **   ** ",
        "**     **",
        "**     **",
        "**     **",
        "**     **",
        "**     **",
        " **   ** ",
        "   ***   ",
    };

    String[] PPattern = {
        "******   ",
        "**    ** ",
        "**     **",
        "**    ** ",
        "******   ",
        "**       ",
        "**       ",
        "**       ",
        "**       ",
    };

    String[] SPattern = {
        "   ***** ",
        " **      ",
        "**       ",
        " **      ",
        "   ***   ",
        "      ** ",
        "       **",
        "      ** ",
        " *****   ",
    };

    String[] SpacePattern = {
        " ",
        " ",
        " ",
        " ",
        " ",
        " ",
        " ",
        " ",
        " ",
    };

    charMaps.put('O', OPattern);
    charMaps.put('P', PPattern);
    charMaps.put('S', SPattern);
    charMaps.put(' ', SpacePattern);

    return charMaps;
  }

  public static void displayBanner(String message, HashMap<Character, String[]> charMap) {
    for (int line = 0; line < 9; line++) {
      StringBuilder sb = new StringBuilder();
      for (char ch : message.toCharArray()) {
        String[] pattern = charMap.get(ch);
        sb.append(pattern[line]).append(" ");
      }
      System.out.println(sb.toString());
    }
  }

  public static void main(String[] args) {
    HashMap<Character, String[]> charMaps = createCharacterMap();

    String message = "OOPS";

    displayBanner(message, charMaps);
  }
}
    }
  }
}
