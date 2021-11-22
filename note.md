  script run cmd: "format": "prettier --single-quote --jsx-single-quote  --jsx-bracket-same-line  --bracket-same-line --trailing-comma all --tab-width 4 --write **/*.{js,json,scss,jsx}",
  //copy to package.json:
  
  "lint-staged": {
        "src/**/*.{js,json,scss,jsx}": "prettier --single-quote --jsx-single-quote  --jsx-bracket-same-line  --bracket-same-line --trailing-comma all --tab-width 4 --write"
    },
    "husky": {
        "hooks": {
            "pre-commit": "lint-staged"
        }
    },
    
      "devDependencies": {
        "husky": "4.3.8",
        "lint-staged": "^12.1.1",
        "prettier": "^2.4.1"
    }
