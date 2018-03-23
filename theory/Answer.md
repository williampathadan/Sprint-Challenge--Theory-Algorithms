## Answers - Theory

### Regular Expressions

1. Single regex that matches

    both `antelope` and `antelopes`

        /antelopes?/g

    both `antelope rocks out` and `antelopes rock out`

        /antelopes?\srocks?\sout/g

2. Regex that matches either of goat, moat but not boat:

        /[gm]oat/g

3. Regex that matches dates in YYYY-MM-DD format.

        /\d{1,4}-\d{1,2}-\d{1,2}/g


### State Machine
* The VT-100 terminal Regex

        /\e\[(1m)?(\d{1,2};\d{1,2}f)?/gi