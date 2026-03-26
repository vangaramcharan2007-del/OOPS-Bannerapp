public class OOPSBannerApp {

  static class CharacterPatternMap {
    Character character;
    String[] pattern;

    public CharacterPatternMap(Character character, String[] pattern) {
      this.character = character;
      this.pattern = pattern;
    }

    public Character getCharacter() {
      return character;
    }

    public String[] getPattern() {
      return pattern;
    }
  }

  public static CharacterPatternMap[] createChracterPatternMaps() {
    CharacterPatternMap[] charMaps = new CharacterPatternMap[4];
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

    charMaps[0] = new CharacterPatternMap('O', OPattern);
    charMaps[1] = new CharacterPatternMap('P', PPattern);
    charMaps[2] = new CharacterPatternMap('S', SPattern);
    charMaps[3] = new CharacterPatternMap(' ', SpacePattern);
    return charMaps;
  }

  public static String[] getCharacterPattern(char ch, CharacterPatternMap[] charMaps) {
    for (CharacterPatternMap map : charMaps) {
      if (map.getCharacter() == ch) {
        return map.getPattern();
      }
    }
    return getCharacterPattern(' ', charMaps);
  }

  public static void printMessage(String message, CharacterPatternMap[] charMaps) {
    for (int i = 0; i < 9; i++) {
      String line = "";
      for (char ch : message.toCharArray()) {
        String[] pattern = getCharacterPattern(ch, charMaps);
        String[] space = getCharacterPattern(' ', charMaps);
        line = line + pattern[i] + space[i];
      }
      System.out.println(line);
    }
  }

  public static void main(String[] args) {
    CharacterPatternMap[] charMaps = createChracterPatternMaps();
    String message = "OOPS";
    printMessage(message, charMaps);
  }
}
