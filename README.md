# tutorial-conan-vs
A tutorial project for using conan package manager within Visual Studio 2017 Community

## Default Profile
```
[settings]
os=Windows
os_build=Windows
arch=x86_64
arch_build=x86_64
compiler=Visual Studio
compiler.version=15
build_type=Release
[options]
[build_requires]
[env]

```

## Install Dependent Packages

```
 conan install .
```

## Visual Studio

```
Open Visual Studio ... set to Release / x64

1>------ Rebuild All started: Project: vs_proj, Configuration: Release x64 ------
1>main.cpp
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-message.h(224): warning C4251: 'testing::Message::ss_': class 'testing::internal::scoped_ptr<std::stringstream>' needs to have dll-interface to be used by clients of class 'testing::Message'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-message.h(224): note: see declaration of 'testing::internal::scoped_ptr<std::stringstream>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-filepath.h(200): warning C4251: 'testing::internal::FilePath::pathname_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::internal::FilePath'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-internal.h(148): warning C4275: non dll-interface class 'std::runtime_error' used as base for dll-interface class 'testing::internal::GoogleTestFailureException'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\stdexcept(157): note: see declaration of 'std::runtime_error'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-internal.h(148): note: see declaration of 'testing::internal::GoogleTestFailureException'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-internal.h(537): warning C4251: 'testing::internal::TypedTestCasePState::defined_test_names_': class 'std::set<const char *,std::less<_Kty>,std::allocator<_Kty>>' needs to have dll-interface to be used by clients of class 'testing::internal::TypedTestCasePState'
1>        with
1>        [
1>            _Kty=const char *
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-internal.h(537): note: see declaration of 'std::set<const char *,std::less<_Kty>,std::allocator<_Kty>>'
1>        with
1>        [
1>            _Kty=const char *
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-death-test-internal.h(134): warning C4251: 'testing::internal::DeathTest::last_death_test_message_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::internal::DeathTest'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(111): warning C4251: 'testing::TestPartResult::file_name_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestPartResult'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(115): warning C4251: 'testing::TestPartResult::summary_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestPartResult'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(116): warning C4251: 'testing::TestPartResult::message_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestPartResult'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(140): warning C4251: 'testing::TestPartResultArray::array_': class 'std::vector<testing::TestPartResult,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestPartResultArray'
1>        with
1>        [
1>            _Ty=testing::TestPartResult
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(140): note: see declaration of 'std::vector<testing::TestPartResult,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=testing::TestPartResult
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(162): warning C4275: non dll-interface class 'testing::TestPartResultReporterInterface' used as base for dll-interface class 'testing::internal::HasNewFatalFailureHelper'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(146): note: see declaration of 'testing::TestPartResultReporterInterface'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(162): note: see declaration of 'testing::internal::HasNewFatalFailureHelper'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(309): warning C4251: 'testing::AssertionResult::message_': class 'testing::internal::scoped_ptr<std::string>' needs to have dll-interface to be used by clients of class 'testing::AssertionResult'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(309): note: see declaration of 'testing::internal::scoped_ptr<std::string>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(595): warning C4251: 'testing::TestResult::test_properites_mutex_': class 'testing::internal::Mutex' needs to have dll-interface to be used by clients of class 'testing::TestResult'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-port.h(1545): note: see declaration of 'testing::internal::Mutex'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(598): warning C4251: 'testing::TestResult::test_part_results_': class 'std::vector<testing::TestPartResult,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestResult'
1>        with
1>        [
1>            _Ty=testing::TestPartResult
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(140): note: see declaration of 'std::vector<testing::TestPartResult,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=testing::TestPartResult
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(600): warning C4251: 'testing::TestResult::test_properties_': class 'std::vector<testing::TestProperty,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestResult'
1>        with
1>        [
1>            _Ty=testing::TestProperty
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(556): note: see declaration of 'std::vector<testing::TestProperty,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=testing::TestProperty
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(720): warning C4251: 'testing::TestInfo::test_case_name_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestInfo'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(721): warning C4251: 'testing::TestInfo::name_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestInfo'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(724): warning C4251: 'testing::TestInfo::type_param_': class 'testing::internal::scoped_ptr<const std::string>' needs to have dll-interface to be used by clients of class 'testing::TestInfo'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(724): note: see declaration of 'testing::internal::scoped_ptr<const std::string>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(727): warning C4251: 'testing::TestInfo::value_param_': class 'testing::internal::scoped_ptr<const std::string>' needs to have dll-interface to be used by clients of class 'testing::TestInfo'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(724): note: see declaration of 'testing::internal::scoped_ptr<const std::string>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(899): warning C4251: 'testing::TestCase::name_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestCase'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(902): warning C4251: 'testing::TestCase::type_param_': class 'testing::internal::scoped_ptr<const std::string>' needs to have dll-interface to be used by clients of class 'testing::TestCase'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(724): note: see declaration of 'testing::internal::scoped_ptr<const std::string>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(905): warning C4251: 'testing::TestCase::test_info_list_': class 'std::vector<testing::TestInfo *,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestCase'
1>        with
1>        [
1>            _Ty=testing::TestInfo *
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(824): note: see declaration of 'std::vector<testing::TestInfo *,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=testing::TestInfo *
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(909): warning C4251: 'testing::TestCase::test_indices_': class 'std::vector<int,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestCase'
1>        with
1>        [
1>            _Ty=int
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(909): note: see declaration of 'std::vector<int,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=int
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(1288): warning C4251: 'testing::UnitTest::mutex_': class 'testing::internal::Mutex' needs to have dll-interface to be used by clients of class 'testing::UnitTest'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-port.h(1545): note: see declaration of 'testing::internal::Mutex'
1>simpleTest.cpp
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-message.h(224): warning C4251: 'testing::Message::ss_': class 'testing::internal::scoped_ptr<std::stringstream>' needs to have dll-interface to be used by clients of class 'testing::Message'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-message.h(224): note: see declaration of 'testing::internal::scoped_ptr<std::stringstream>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-filepath.h(200): warning C4251: 'testing::internal::FilePath::pathname_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::internal::FilePath'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-internal.h(148): warning C4275: non dll-interface class 'std::runtime_error' used as base for dll-interface class 'testing::internal::GoogleTestFailureException'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\stdexcept(157): note: see declaration of 'std::runtime_error'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-internal.h(148): note: see declaration of 'testing::internal::GoogleTestFailureException'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-internal.h(537): warning C4251: 'testing::internal::TypedTestCasePState::defined_test_names_': class 'std::set<const char *,std::less<_Kty>,std::allocator<_Kty>>' needs to have dll-interface to be used by clients of class 'testing::internal::TypedTestCasePState'
1>        with
1>        [
1>            _Kty=const char *
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-internal.h(537): note: see declaration of 'std::set<const char *,std::less<_Kty>,std::allocator<_Kty>>'
1>        with
1>        [
1>            _Kty=const char *
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-death-test-internal.h(134): warning C4251: 'testing::internal::DeathTest::last_death_test_message_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::internal::DeathTest'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(111): warning C4251: 'testing::TestPartResult::file_name_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestPartResult'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(115): warning C4251: 'testing::TestPartResult::summary_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestPartResult'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(116): warning C4251: 'testing::TestPartResult::message_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestPartResult'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(140): warning C4251: 'testing::TestPartResultArray::array_': class 'std::vector<testing::TestPartResult,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestPartResultArray'
1>        with
1>        [
1>            _Ty=testing::TestPartResult
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(140): note: see declaration of 'std::vector<testing::TestPartResult,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=testing::TestPartResult
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(162): warning C4275: non dll-interface class 'testing::TestPartResultReporterInterface' used as base for dll-interface class 'testing::internal::HasNewFatalFailureHelper'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(146): note: see declaration of 'testing::TestPartResultReporterInterface'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(162): note: see declaration of 'testing::internal::HasNewFatalFailureHelper'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(309): warning C4251: 'testing::AssertionResult::message_': class 'testing::internal::scoped_ptr<std::string>' needs to have dll-interface to be used by clients of class 'testing::AssertionResult'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(309): note: see declaration of 'testing::internal::scoped_ptr<std::string>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(595): warning C4251: 'testing::TestResult::test_properites_mutex_': class 'testing::internal::Mutex' needs to have dll-interface to be used by clients of class 'testing::TestResult'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-port.h(1545): note: see declaration of 'testing::internal::Mutex'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(598): warning C4251: 'testing::TestResult::test_part_results_': class 'std::vector<testing::TestPartResult,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestResult'
1>        with
1>        [
1>            _Ty=testing::TestPartResult
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest-test-part.h(140): note: see declaration of 'std::vector<testing::TestPartResult,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=testing::TestPartResult
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(600): warning C4251: 'testing::TestResult::test_properties_': class 'std::vector<testing::TestProperty,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestResult'
1>        with
1>        [
1>            _Ty=testing::TestProperty
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(556): note: see declaration of 'std::vector<testing::TestProperty,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=testing::TestProperty
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(720): warning C4251: 'testing::TestInfo::test_case_name_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestInfo'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(721): warning C4251: 'testing::TestInfo::name_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestInfo'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(724): warning C4251: 'testing::TestInfo::type_param_': class 'testing::internal::scoped_ptr<const std::string>' needs to have dll-interface to be used by clients of class 'testing::TestInfo'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(724): note: see declaration of 'testing::internal::scoped_ptr<const std::string>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(727): warning C4251: 'testing::TestInfo::value_param_': class 'testing::internal::scoped_ptr<const std::string>' needs to have dll-interface to be used by clients of class 'testing::TestInfo'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(724): note: see declaration of 'testing::internal::scoped_ptr<const std::string>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(899): warning C4251: 'testing::TestCase::name_': class 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>' needs to have dll-interface to be used by clients of class 'testing::TestCase'
1>D:\Programs\Microsoft Visual Studio\2017\Community\VC\Tools\MSVC\14.10.25017\include\xstring(3997): note: see declaration of 'std::basic_string<char,std::char_traits<char>,std::allocator<char>>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(902): warning C4251: 'testing::TestCase::type_param_': class 'testing::internal::scoped_ptr<const std::string>' needs to have dll-interface to be used by clients of class 'testing::TestCase'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(724): note: see declaration of 'testing::internal::scoped_ptr<const std::string>'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(905): warning C4251: 'testing::TestCase::test_info_list_': class 'std::vector<testing::TestInfo *,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestCase'
1>        with
1>        [
1>            _Ty=testing::TestInfo *
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(824): note: see declaration of 'std::vector<testing::TestInfo *,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=testing::TestInfo *
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(909): warning C4251: 'testing::TestCase::test_indices_': class 'std::vector<int,std::allocator<_Ty>>' needs to have dll-interface to be used by clients of class 'testing::TestCase'
1>        with
1>        [
1>            _Ty=int
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(909): note: see declaration of 'std::vector<int,std::allocator<_Ty>>'
1>        with
1>        [
1>            _Ty=int
1>        ]
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/gtest.h(1288): warning C4251: 'testing::UnitTest::mutex_': class 'testing::internal::Mutex' needs to have dll-interface to be used by clients of class 'testing::UnitTest'
1>C:\Users\Eric\.conan\data\gtest\1.7.0\bincrafters\stable\package\970e773c5651dc2560f86200a4ea56c23f568ff9\include\gtest/internal/gtest-port.h(1545): note: see declaration of 'testing::internal::Mutex'
1>Generating code
1>All 14 functions were compiled because no usable IPDB/IOBJ from previous compilation was found.
1>Finished generating code
1>vs_proj.vcxproj -> D:\Projects\conan\tutorial-conan-vs\vs_proj\x64\Release\vs_proj.exe
1>Done building project "vs_proj.vcxproj".
========== Rebuild All: 1 succeeded, 0 failed, 0 skipped ==========

```

## Output Log
```
conan install .
gtest/1.7.0@bincrafters/stable: Not found in local cache, looking in remotes...
gtest/1.7.0@bincrafters/stable: Trying with 'conan-center'...
Downloading conanmanifest.txt
[==================================================] 166B/166B
Downloading conanfile.py
[==================================================] 2.5KB/2.5KB
Downloading conan_export.tgz
[==================================================] 758B/758B
PROJECT: Installing D:\Projects\conan\test6\conanfile.txt
Requirements
    gtest/1.7.0@bincrafters/stable from 'conan-center' - Downloaded
Packages
    gtest/1.7.0@bincrafters/stable:970e773c5651dc2560f86200a4ea56c23f568ff9 - Download

gtest/1.7.0@bincrafters/stable: Retrieving package 970e773c5651dc2560f86200a4ea56c23f568ff9 from remote 'conan-center'
Downloading conanmanifest.txt
[==================================================] 1.8KB/1.8KB
Downloading conaninfo.txt
[==================================================] 436B/436B
Downloading conan_package.tgz
[==================================================] 449.2KB/449.2KB
gtest/1.7.0@bincrafters/stable: Package installed 970e773c5651dc2560f86200a4ea56c23f568ff9
PROJECT: Generator visual_studio_multi created conanbuildinfo_multi.props
PROJECT: Generator visual_studio_multi created conanbuildinfo_release_x64_v141.props
PROJECT: Generator txt created conanbuildinfo.txt
PROJECT: Generated conaninfo.txt
```