tasks 51 
public class NumberStringUtil {
    public boolean isNumber(String str) {
        return str.matches("\d+");
    }
}

import static org.junit.jupiter.api.Assertions.assertTrue;
import org.junit.jupiter.api.Test;

public class NumberStringUtilTest {
    @Test
    public void testIsNumber() {
        NumberStringUtil numberStringUtil = new NumberStringUtil();
        assertTrue(numberStringUtil.isNumber("123456"));
        assertFalse(numberStringUtil.isNumber("123a"));
    }
}

tasks 52
public class CorrectorUtil {
    public String correctString(String str) {
        return str.replace('o', '0');
    }
}

import static org.junit.jupiter.api.Assertions.assertEquals;
import org.junit.jupiter.api.Test;

public class CorrectorUtilTest {
    @Test
    public void testCorrectString() {
        CorrectorUtil correctorUtil = new CorrectorUtil();
        assertEquals("H3ll0 W0rld", correctorUtil.correctString("Hello World"));
    }
}
