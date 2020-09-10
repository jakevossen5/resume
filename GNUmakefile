all : resume.pdf jake-vossen-resume.pdf jake-vossen-cv.pdf cover-letters/cover-letter-generic.pdf cover-letters/cover-letter-google.pdf cover-letters/cover-letter-onepassword.pdf

clean:
	rm *.pdf || true
	rm __latexindent_temp* || true
	rm cv/__latexindent_temp* || true
	rm *.aux || true
	rm *.log || true
	rm *.out || true
	rm *.synctex.* || true

jake-vossen-cv.pdf : fonts/FontAwesome.ttf fonts/Roboto-Bold.ttf fonts/Roboto-BoldItalic.ttf fonts/Roboto-Italic.ttf fonts/Roboto-Light.ttf fonts/Roboto-LightItalic.ttf fonts/Roboto-Medium.ttf fonts/Roboto-MediumItalic.ttf fonts/Roboto-Regular.ttf fonts/Roboto-Thin.ttf fonts/Roboto-ThinItalic.ttf awesome-cv.cls fontawesome.sty cv/education.tex cv/experience.tex cv/skills.tex cv.tex cv/honors.tex cv/extracurricular.tex base.tex

	xelatex cv.tex
	mv cv.pdf jake-vossen-cv.pdf

jake-vossen-resume.pdf : resume.pdf
	cp resume.pdf jake-vossen-resume.pdf

resume.pdf : fonts/FontAwesome.ttf fonts/Roboto-Bold.ttf fonts/Roboto-BoldItalic.ttf fonts/Roboto-Italic.ttf fonts/Roboto-Light.ttf fonts/Roboto-LightItalic.ttf fonts/Roboto-Medium.ttf fonts/Roboto-MediumItalic.ttf fonts/Roboto-Regular.ttf fonts/Roboto-Thin.ttf fonts/Roboto-ThinItalic.ttf awesome-cv.cls fontawesome.sty cv/education.tex cv/experience.tex cv/skills.tex cv.tex cv/honors.tex cv/extracurricular.tex base.tex
	xelatex resume.tex

cover-letters/cover-letter-generic.pdf : cover-letter-generic.tex cover-letter.tex why-generic.tex
	xelatex cover-letter-generic.tex
	mv cover-letter-generic.pdf cover-letters/cover-letter-generic.pdf

cover-letters/cover-letter-onepassword.pdf : cover-letter-onepassword.tex cover-letter.tex why-onepassword.tex
	xelatex cover-letter-onepassword.tex
	mv cover-letter-onepassword.pdf cover-letters/cover-letter-onepassword.pdf

cover-letters/cover-letter-google.pdf : cover-letter-google.tex cover-letter.tex
	xelatex cover-letter-google.tex
	mv cover-letter-google.pdf cover-letters/cover-letter-google.pdf
