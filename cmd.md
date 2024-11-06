

```cmd
python -c "import shutil, os; shutil.rmtree('build') if os.path.exists('build') else print('Directory does not exist')"
python -c "import shutil, os; shutil.rmtree('dist') if os.path.exists('dist') else print('Directory does not exist')"
python setup.py sdist build
python setup.py sdist bdist_wheel
python -m twine upload dist/*   
pip uninstall DrissionPage
pip install dist/PlayDrissionPage-0.0.1.3.tar.gz
```