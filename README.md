Modified to fix enumeration.

When call words_for(nil, x, y, width, height) the tesseract engine was erroring out and behaving unpredictably.

Fixed this by commenting out various parts of tesseract/engine/iterator.rb. This prevents some calls to the tesseract c library which seems to fix the issue. 