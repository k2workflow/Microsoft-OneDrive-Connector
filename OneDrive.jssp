(function () {
    function asyncGeneratorStep(gen, resolve, reject, _next, _throw, key, arg) {
        try {
            var info = gen[key](arg);
            var value = info.value;
        } catch (error) {
            reject(error);
            return;
        }

        if (info.done) {
            resolve(value);
        } else {
            Promise.resolve(value).then(_next, _throw);
        }
    }

    function _asyncToGenerator(fn) {
        return function () {
            var self = this,
                args = arguments;
            return new Promise(function (resolve, reject) {
                var gen = fn.apply(self, args);

                function _next(value) {
                    asyncGeneratorStep(gen, resolve, reject, _next, _throw, "next", value);
                }

                function _throw(err) {
                    asyncGeneratorStep(gen, resolve, reject, _next, _throw, "throw", err);
                }

                _next(undefined);
            });
        };
    }

    function _classCallCheck(instance, Constructor) {
        if (!(instance instanceof Constructor)) {
            throw new TypeError("Cannot call a class as a function");
        }
    }

    function _defineProperties(target, props) {
        for (var i = 0; i < props.length; i++) {
            var descriptor = props[i];
            descriptor.enumerable = descriptor.enumerable || false;
            descriptor.configurable = true;
            if ("value" in descriptor) descriptor.writable = true;
            Object.defineProperty(target, descriptor.key, descriptor);
        }
    }

    function _createClass(Constructor, protoProps, staticProps) {
        if (protoProps) _defineProperties(Constructor.prototype, protoProps);
        if (staticProps) _defineProperties(Constructor, staticProps);
        return Constructor;
    }

    function _defineProperty(obj, key, value) {
        if (key in obj) {
            Object.defineProperty(obj, key, {
                value: value,
                enumerable: true,
                configurable: true,
                writable: true
            });
        } else {
            obj[key] = value;
        }

        return obj;
    }

    function ownKeys(object, enumerableOnly) {
        var keys = Object.keys(object);

        if (Object.getOwnPropertySymbols) {
            var symbols = Object.getOwnPropertySymbols(object);
            if (enumerableOnly) symbols = symbols.filter(function (sym) {
                return Object.getOwnPropertyDescriptor(object, sym).enumerable;
            });
            keys.push.apply(keys, symbols);
        }

        return keys;
    }

    function _objectSpread2(target) {
        for (var i = 1; i < arguments.length; i++) {
            var source = arguments[i] != null ? arguments[i] : {};

            if (i % 2) {
                ownKeys(Object(source), true).forEach(function (key) {
                    _defineProperty(target, key, source[key]);
                });
            } else if (Object.getOwnPropertyDescriptors) {
                Object.defineProperties(target, Object.getOwnPropertyDescriptors(source));
            } else {
                ownKeys(Object(source)).forEach(function (key) {
                    Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key));
                });
            }
        }

        return target;
    }

    function _inherits(subClass, superClass) {
        if (typeof superClass !== "function" && superClass !== null) {
            throw new TypeError("Super expression must either be null or a function");
        }

        subClass.prototype = Object.create(superClass && superClass.prototype, {
            constructor: {
                value: subClass,
                writable: true,
                configurable: true
            }
        });
        if (superClass) _setPrototypeOf(subClass, superClass);
    }

    function _getPrototypeOf(o) {
        _getPrototypeOf = Object.setPrototypeOf ? Object.getPrototypeOf : function _getPrototypeOf(o) {
            return o.__proto__ || Object.getPrototypeOf(o);
        };
        return _getPrototypeOf(o);
    }

    function _setPrototypeOf(o, p) {
        _setPrototypeOf = Object.setPrototypeOf || function _setPrototypeOf(o, p) {
            o.__proto__ = p;
            return o;
        };

        return _setPrototypeOf(o, p);
    }

    function _isNativeReflectConstruct() {
        if (typeof Reflect === "undefined" || !Reflect.construct) return false;
        if (Reflect.construct.sham) return false;
        if (typeof Proxy === "function") return true;

        try {
            Date.prototype.toString.call(Reflect.construct(Date, [], function () {}));
            return true;
        } catch (e) {
            return false;
        }
    }

    function _assertThisInitialized(self) {
        if (self === void 0) {
            throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
        }

        return self;
    }

    function _possibleConstructorReturn(self, call) {
        if (call && (typeof call === "object" || typeof call === "function")) {
            return call;
        }

        return _assertThisInitialized(self);
    }

    function _createSuper(Derived) {
        return function () {
            var Super = _getPrototypeOf(Derived),
                result;

            if (_isNativeReflectConstruct()) {
                var NewTarget = _getPrototypeOf(this).constructor;

                result = Reflect.construct(Super, arguments, NewTarget);
            } else {
                result = Super.apply(this, arguments);
            }

            return _possibleConstructorReturn(this, result);
        };
    }

    function _unsupportedIterableToArray(o, minLen) {
        if (!o) return;
        if (typeof o === "string") return _arrayLikeToArray(o, minLen);
        var n = Object.prototype.toString.call(o).slice(8, -1);
        if (n === "Object" && o.constructor) n = o.constructor.name;
        if (n === "Map" || n === "Set") return Array.from(n);
        if (n === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return _arrayLikeToArray(o, minLen);
    }

    function _arrayLikeToArray(arr, len) {
        if (len == null || len > arr.length) len = arr.length;

        for (var i = 0, arr2 = new Array(len); i < len; i++) arr2[i] = arr[i];

        return arr2;
    }

    function _createForOfIteratorHelper(o) {
        if (typeof Symbol === "undefined" || o[Symbol.iterator] == null) {
            if (Array.isArray(o) || (o = _unsupportedIterableToArray(o))) {
                var i = 0;

                var F = function () {};

                return {
                    s: F,
                    n: function () {
                        if (i >= o.length) return {
                            done: true
                        };
                        return {
                            done: false,
                            value: o[i++]
                        };
                    },
                    e: function (e) {
                        throw e;
                    },
                    f: F
                };
            }

            throw new TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.");
        }

        var it,
            normalCompletion = true,
            didErr = false,
            err;
        return {
            s: function () {
                it = o[Symbol.iterator]();
            },
            n: function () {
                var step = it.next();
                normalCompletion = step.done;
                return step;
            },
            e: function (e) {
                didErr = true;
                err = e;
            },
            f: function () {
                try {
                    if (!normalCompletion && it.return != null) it.return();
                } finally {
                    if (didErr) throw err;
                }
            }
        };
    }

    var commonjsGlobal = typeof globalThis !== 'undefined' ? globalThis : typeof window !== 'undefined' ? window : typeof global !== 'undefined' ? global : typeof self !== 'undefined' ? self : {};

    function createCommonjsModule(fn, module) {
        return module = { exports: {} }, fn(module, module.exports), module.exports;
    }

    var runtime_1 = createCommonjsModule(function (module) {
        /**
         * Copyright (c) 2014-present, Facebook, Inc.
         *
         * This source code is licensed under the MIT license found in the
         * LICENSE file in the root directory of this source tree.
         */
        var runtime = function (exports) {

            var Op = Object.prototype;
            var hasOwn = Op.hasOwnProperty;
            var undefined$1; // More compressible than void 0.

            var $Symbol = typeof Symbol === "function" ? Symbol : {};
            var iteratorSymbol = $Symbol.iterator || "@@iterator";
            var asyncIteratorSymbol = $Symbol.asyncIterator || "@@asyncIterator";
            var toStringTagSymbol = $Symbol.toStringTag || "@@toStringTag";

            function wrap(innerFn, outerFn, self, tryLocsList) {
                // If outerFn provided and outerFn.prototype is a Generator, then outerFn.prototype instanceof Generator.
                var protoGenerator = outerFn && outerFn.prototype instanceof Generator ? outerFn : Generator;
                var generator = Object.create(protoGenerator.prototype);
                var context = new Context(tryLocsList || []); // The ._invoke method unifies the implementations of the .next,
                // .throw, and .return methods.

                generator._invoke = makeInvokeMethod(innerFn, self, context);
                return generator;
            }

            exports.wrap = wrap; // Try/catch helper to minimize deoptimizations. Returns a completion
            // record like context.tryEntries[i].completion. This interface could
            // have been (and was previously) designed to take a closure to be
            // invoked without arguments, but in all the cases we care about we
            // already have an existing method we want to call, so there's no need
            // to create a new function object. We can even get away with assuming
            // the method takes exactly one argument, since that happens to be true
            // in every case, so we don't have to touch the arguments object. The
            // only additional allocation required is the completion record, which
            // has a stable shape and so hopefully should be cheap to allocate.

            function tryCatch(fn, obj, arg) {
                try {
                    return {
                        type: "normal",
                        arg: fn.call(obj, arg)
                    };
                } catch (err) {
                    return {
                        type: "throw",
                        arg: err
                    };
                }
            }

            var GenStateSuspendedStart = "suspendedStart";
            var GenStateSuspendedYield = "suspendedYield";
            var GenStateExecuting = "executing";
            var GenStateCompleted = "completed"; // Returning this object from the innerFn has the same effect as
            // breaking out of the dispatch switch statement.

            var ContinueSentinel = {}; // Dummy constructor functions that we use as the .constructor and
            // .constructor.prototype properties for functions that return Generator
            // objects. For full spec compliance, you may wish to configure your
            // minifier not to mangle the names of these two functions.

            function Generator() {}

            function GeneratorFunction() {}

            function GeneratorFunctionPrototype() {} // This is a polyfill for %IteratorPrototype% for environments that
            // don't natively support it.


            var IteratorPrototype = {};

            IteratorPrototype[iteratorSymbol] = function () {
                return this;
            };

            var getProto = Object.getPrototypeOf;
            var NativeIteratorPrototype = getProto && getProto(getProto(values([])));

            if (NativeIteratorPrototype && NativeIteratorPrototype !== Op && hasOwn.call(NativeIteratorPrototype, iteratorSymbol)) {
                // This environment has a native %IteratorPrototype%; use it instead
                // of the polyfill.
                IteratorPrototype = NativeIteratorPrototype;
            }

            var Gp = GeneratorFunctionPrototype.prototype = Generator.prototype = Object.create(IteratorPrototype);
            GeneratorFunction.prototype = Gp.constructor = GeneratorFunctionPrototype;
            GeneratorFunctionPrototype.constructor = GeneratorFunction;
            GeneratorFunctionPrototype[toStringTagSymbol] = GeneratorFunction.displayName = "GeneratorFunction"; // Helper for defining the .next, .throw, and .return methods of the
            // Iterator interface in terms of a single ._invoke method.

            function defineIteratorMethods(prototype) {
                ["next", "throw", "return"].forEach(function (method) {
                    prototype[method] = function (arg) {
                        return this._invoke(method, arg);
                    };
                });
            }

            exports.isGeneratorFunction = function (genFun) {
                var ctor = typeof genFun === "function" && genFun.constructor;
                return ctor ? ctor === GeneratorFunction || // For the native GeneratorFunction constructor, the best we can
                    // do is to check its .name property.
                    (ctor.displayName || ctor.name) === "GeneratorFunction" : false;
            };

            exports.mark = function (genFun) {
                if (Object.setPrototypeOf) {
                    Object.setPrototypeOf(genFun, GeneratorFunctionPrototype);
                } else {
                    genFun.__proto__ = GeneratorFunctionPrototype;

                    if (!(toStringTagSymbol in genFun)) {
                        genFun[toStringTagSymbol] = "GeneratorFunction";
                    }
                }

                genFun.prototype = Object.create(Gp);
                return genFun;
            }; // Within the body of any async function, `await x` is transformed to
            // `yield regeneratorRuntime.awrap(x)`, so that the runtime can test
            // `hasOwn.call(value, "__await")` to determine if the yielded value is
            // meant to be awaited.


            exports.awrap = function (arg) {
                return {
                    __await: arg
                };
            };

            function AsyncIterator(generator, PromiseImpl) {
                function invoke(method, arg, resolve, reject) {
                    var record = tryCatch(generator[method], generator, arg);

                    if (record.type === "throw") {
                        reject(record.arg);
                    } else {
                        var result = record.arg;
                        var value = result.value;

                        if (value && typeof value === "object" && hasOwn.call(value, "__await")) {
                            return PromiseImpl.resolve(value.__await).then(function (value) {
                                invoke("next", value, resolve, reject);
                            }, function (err) {
                                invoke("throw", err, resolve, reject);
                            });
                        }

                        return PromiseImpl.resolve(value).then(function (unwrapped) {
                            // When a yielded Promise is resolved, its final value becomes
                            // the .value of the Promise<{value,done}> result for the
                            // current iteration.
                            result.value = unwrapped;
                            resolve(result);
                        }, function (error) {
                            // If a rejected Promise was yielded, throw the rejection back
                            // into the async generator function so it can be handled there.
                            return invoke("throw", error, resolve, reject);
                        });
                    }
                }

                var previousPromise;

                function enqueue(method, arg) {
                    function callInvokeWithMethodAndArg() {
                        return new PromiseImpl(function (resolve, reject) {
                            invoke(method, arg, resolve, reject);
                        });
                    }

                    return previousPromise = // If enqueue has been called before, then we want to wait until
                        // all previous Promises have been resolved before calling invoke,
                        // so that results are always delivered in the correct order. If
                        // enqueue has not been called before, then it is important to
                        // call invoke immediately, without waiting on a callback to fire,
                        // so that the async generator function has the opportunity to do
                        // any necessary setup in a predictable way. This predictability
                        // is why the Promise constructor synchronously invokes its
                        // executor callback, and why async functions synchronously
                        // execute code before the first await. Since we implement simple
                        // async functions in terms of async generators, it is especially
                        // important to get this right, even though it requires care.
                        previousPromise ? previousPromise.then(callInvokeWithMethodAndArg, // Avoid propagating failures to Promises returned by later
                            // invocations of the iterator.
                            callInvokeWithMethodAndArg) : callInvokeWithMethodAndArg();
                } // Define the unified helper method that is used to implement .next,
                // .throw, and .return (see defineIteratorMethods).


                this._invoke = enqueue;
            }

            defineIteratorMethods(AsyncIterator.prototype);

            AsyncIterator.prototype[asyncIteratorSymbol] = function () {
                return this;
            };

            exports.AsyncIterator = AsyncIterator; // Note that simple async functions are implemented on top of
            // AsyncIterator objects; they just return a Promise for the value of
            // the final result produced by the iterator.

            exports.async = function (innerFn, outerFn, self, tryLocsList, PromiseImpl) {
                if (PromiseImpl === void 0) PromiseImpl = Promise;
                var iter = new AsyncIterator(wrap(innerFn, outerFn, self, tryLocsList), PromiseImpl);
                return exports.isGeneratorFunction(outerFn) ? iter // If outerFn is a generator, return the full iterator.
                    : iter.next().then(function (result) {
                        return result.done ? result.value : iter.next();
                    });
            };

            function makeInvokeMethod(innerFn, self, context) {
                var state = GenStateSuspendedStart;
                return function invoke(method, arg) {
                    if (state === GenStateExecuting) {
                        throw new Error("Generator is already running");
                    }

                    if (state === GenStateCompleted) {
                        if (method === "throw") {
                            throw arg;
                        } // Be forgiving, per 25.3.3.3.3 of the spec:
                        // https://people.mozilla.org/~jorendorff/es6-draft.html#sec-generatorresume


                        return doneResult();
                    }

                    context.method = method;
                    context.arg = arg;

                    while (true) {
                        var delegate = context.delegate;

                        if (delegate) {
                            var delegateResult = maybeInvokeDelegate(delegate, context);

                            if (delegateResult) {
                                if (delegateResult === ContinueSentinel) continue;
                                return delegateResult;
                            }
                        }

                        if (context.method === "next") {
                            // Setting context._sent for legacy support of Babel's
                            // function.sent implementation.
                            context.sent = context._sent = context.arg;
                        } else if (context.method === "throw") {
                            if (state === GenStateSuspendedStart) {
                                state = GenStateCompleted;
                                throw context.arg;
                            }

                            context.dispatchException(context.arg);
                        } else if (context.method === "return") {
                            context.abrupt("return", context.arg);
                        }

                        state = GenStateExecuting;
                        var record = tryCatch(innerFn, self, context);

                        if (record.type === "normal") {
                            // If an exception is thrown from innerFn, we leave state ===
                            // GenStateExecuting and loop back for another invocation.
                            state = context.done ? GenStateCompleted : GenStateSuspendedYield;

                            if (record.arg === ContinueSentinel) {
                                continue;
                            }

                            return {
                                value: record.arg,
                                done: context.done
                            };
                        } else if (record.type === "throw") {
                            state = GenStateCompleted; // Dispatch the exception by looping back around to the
                            // context.dispatchException(context.arg) call above.

                            context.method = "throw";
                            context.arg = record.arg;
                        }
                    }
                };
            } // Call delegate.iterator[context.method](context.arg) and handle the
            // result, either by returning a { value, done } result from the
            // delegate iterator, or by modifying context.method and context.arg,
            // setting context.delegate to null, and returning the ContinueSentinel.


            function maybeInvokeDelegate(delegate, context) {
                var method = delegate.iterator[context.method];

                if (method === undefined$1) {
                    // A .throw or .return when the delegate iterator has no .throw
                    // method always terminates the yield* loop.
                    context.delegate = null;

                    if (context.method === "throw") {
                        // Note: ["return"] must be used for ES3 parsing compatibility.
                        if (delegate.iterator["return"]) {
                            // If the delegate iterator has a return method, give it a
                            // chance to clean up.
                            context.method = "return";
                            context.arg = undefined$1;
                            maybeInvokeDelegate(delegate, context);

                            if (context.method === "throw") {
                                // If maybeInvokeDelegate(context) changed context.method from
                                // "return" to "throw", let that override the TypeError below.
                                return ContinueSentinel;
                            }
                        }

                        context.method = "throw";
                        context.arg = new TypeError("The iterator does not provide a 'throw' method");
                    }

                    return ContinueSentinel;
                }

                var record = tryCatch(method, delegate.iterator, context.arg);

                if (record.type === "throw") {
                    context.method = "throw";
                    context.arg = record.arg;
                    context.delegate = null;
                    return ContinueSentinel;
                }

                var info = record.arg;

                if (!info) {
                    context.method = "throw";
                    context.arg = new TypeError("iterator result is not an object");
                    context.delegate = null;
                    return ContinueSentinel;
                }

                if (info.done) {
                    // Assign the result of the finished delegate to the temporary
                    // variable specified by delegate.resultName (see delegateYield).
                    context[delegate.resultName] = info.value; // Resume execution at the desired location (see delegateYield).

                    context.next = delegate.nextLoc; // If context.method was "throw" but the delegate handled the
                    // exception, let the outer generator proceed normally. If
                    // context.method was "next", forget context.arg since it has been
                    // "consumed" by the delegate iterator. If context.method was
                    // "return", allow the original .return call to continue in the
                    // outer generator.

                    if (context.method !== "return") {
                        context.method = "next";
                        context.arg = undefined$1;
                    }
                } else {
                    // Re-yield the result returned by the delegate method.
                    return info;
                } // The delegate iterator is finished, so forget it and continue with
                // the outer generator.


                context.delegate = null;
                return ContinueSentinel;
            } // Define Generator.prototype.{next,throw,return} in terms of the
            // unified ._invoke helper method.


            defineIteratorMethods(Gp);
            Gp[toStringTagSymbol] = "Generator"; // A Generator should always return itself as the iterator object when the
            // @@iterator function is called on it. Some browsers' implementations of the
            // iterator prototype chain incorrectly implement this, causing the Generator
            // object to not be returned from this call. This ensures that doesn't happen.
            // See https://github.com/facebook/regenerator/issues/274 for more details.

            Gp[iteratorSymbol] = function () {
                return this;
            };

            Gp.toString = function () {
                return "[object Generator]";
            };

            function pushTryEntry(locs) {
                var entry = {
                    tryLoc: locs[0]
                };

                if (1 in locs) {
                    entry.catchLoc = locs[1];
                }

                if (2 in locs) {
                    entry.finallyLoc = locs[2];
                    entry.afterLoc = locs[3];
                }

                this.tryEntries.push(entry);
            }

            function resetTryEntry(entry) {
                var record = entry.completion || {};
                record.type = "normal";
                delete record.arg;
                entry.completion = record;
            }

            function Context(tryLocsList) {
                // The root entry object (effectively a try statement without a catch
                // or a finally block) gives us a place to store values thrown from
                // locations where there is no enclosing try statement.
                this.tryEntries = [{
                    tryLoc: "root"
                }];
                tryLocsList.forEach(pushTryEntry, this);
                this.reset(true);
            }

            exports.keys = function (object) {
                var keys = [];

                for (var key in object) {
                    keys.push(key);
                }

                keys.reverse(); // Rather than returning an object with a next method, we keep
                // things simple and return the next function itself.

                return function next() {
                    while (keys.length) {
                        var key = keys.pop();

                        if (key in object) {
                            next.value = key;
                            next.done = false;
                            return next;
                        }
                    } // To avoid creating an additional object, we just hang the .value
                    // and .done properties off the next function object itself. This
                    // also ensures that the minifier will not anonymize the function.


                    next.done = true;
                    return next;
                };
            };

            function values(iterable) {
                if (iterable) {
                    var iteratorMethod = iterable[iteratorSymbol];

                    if (iteratorMethod) {
                        return iteratorMethod.call(iterable);
                    }

                    if (typeof iterable.next === "function") {
                        return iterable;
                    }

                    if (!isNaN(iterable.length)) {
                        var i = -1,
                            next = function next() {
                                while (++i < iterable.length) {
                                    if (hasOwn.call(iterable, i)) {
                                        next.value = iterable[i];
                                        next.done = false;
                                        return next;
                                    }
                                }

                                next.value = undefined$1;
                                next.done = true;
                                return next;
                            };

                        return next.next = next;
                    }
                } // Return an iterator with no values.


                return {
                    next: doneResult
                };
            }

            exports.values = values;

            function doneResult() {
                return {
                    value: undefined$1,
                    done: true
                };
            }

            Context.prototype = {
                constructor: Context,
                reset: function (skipTempReset) {
                    this.prev = 0;
                    this.next = 0; // Resetting context._sent for legacy support of Babel's
                    // function.sent implementation.

                    this.sent = this._sent = undefined$1;
                    this.done = false;
                    this.delegate = null;
                    this.method = "next";
                    this.arg = undefined$1;
                    this.tryEntries.forEach(resetTryEntry);

                    if (!skipTempReset) {
                        for (var name in this) {
                            // Not sure about the optimal order of these conditions:
                            if (name.charAt(0) === "t" && hasOwn.call(this, name) && !isNaN(+name.slice(1))) {
                                this[name] = undefined$1;
                            }
                        }
                    }
                },
                stop: function () {
                    this.done = true;
                    var rootEntry = this.tryEntries[0];
                    var rootRecord = rootEntry.completion;

                    if (rootRecord.type === "throw") {
                        throw rootRecord.arg;
                    }

                    return this.rval;
                },
                dispatchException: function (exception) {
                    if (this.done) {
                        throw exception;
                    }

                    var context = this;

                    function handle(loc, caught) {
                        record.type = "throw";
                        record.arg = exception;
                        context.next = loc;

                        if (caught) {
                            // If the dispatched exception was caught by a catch block,
                            // then let that catch block handle the exception normally.
                            context.method = "next";
                            context.arg = undefined$1;
                        }

                        return !!caught;
                    }

                    for (var i = this.tryEntries.length - 1; i >= 0; --i) {
                        var entry = this.tryEntries[i];
                        var record = entry.completion;

                        if (entry.tryLoc === "root") {
                            // Exception thrown outside of any try block that could handle
                            // it, so set the completion value of the entire function to
                            // throw the exception.
                            return handle("end");
                        }

                        if (entry.tryLoc <= this.prev) {
                            var hasCatch = hasOwn.call(entry, "catchLoc");
                            var hasFinally = hasOwn.call(entry, "finallyLoc");

                            if (hasCatch && hasFinally) {
                                if (this.prev < entry.catchLoc) {
                                    return handle(entry.catchLoc, true);
                                } else if (this.prev < entry.finallyLoc) {
                                    return handle(entry.finallyLoc);
                                }
                            } else if (hasCatch) {
                                if (this.prev < entry.catchLoc) {
                                    return handle(entry.catchLoc, true);
                                }
                            } else if (hasFinally) {
                                if (this.prev < entry.finallyLoc) {
                                    return handle(entry.finallyLoc);
                                }
                            } else {
                                throw new Error("try statement without catch or finally");
                            }
                        }
                    }
                },
                abrupt: function (type, arg) {
                    for (var i = this.tryEntries.length - 1; i >= 0; --i) {
                        var entry = this.tryEntries[i];

                        if (entry.tryLoc <= this.prev && hasOwn.call(entry, "finallyLoc") && this.prev < entry.finallyLoc) {
                            var finallyEntry = entry;
                            break;
                        }
                    }

                    if (finallyEntry && (type === "break" || type === "continue") && finallyEntry.tryLoc <= arg && arg <= finallyEntry.finallyLoc) {
                        // Ignore the finally entry if control is not jumping to a
                        // location outside the try/catch block.
                        finallyEntry = null;
                    }

                    var record = finallyEntry ? finallyEntry.completion : {};
                    record.type = type;
                    record.arg = arg;

                    if (finallyEntry) {
                        this.method = "next";
                        this.next = finallyEntry.finallyLoc;
                        return ContinueSentinel;
                    }

                    return this.complete(record);
                },
                complete: function (record, afterLoc) {
                    if (record.type === "throw") {
                        throw record.arg;
                    }

                    if (record.type === "break" || record.type === "continue") {
                        this.next = record.arg;
                    } else if (record.type === "return") {
                        this.rval = this.arg = record.arg;
                        this.method = "return";
                        this.next = "end";
                    } else if (record.type === "normal" && afterLoc) {
                        this.next = afterLoc;
                    }

                    return ContinueSentinel;
                },
                finish: function (finallyLoc) {
                    for (var i = this.tryEntries.length - 1; i >= 0; --i) {
                        var entry = this.tryEntries[i];

                        if (entry.finallyLoc === finallyLoc) {
                            this.complete(entry.completion, entry.afterLoc);
                            resetTryEntry(entry);
                            return ContinueSentinel;
                        }
                    }
                },
                "catch": function (tryLoc) {
                    for (var i = this.tryEntries.length - 1; i >= 0; --i) {
                        var entry = this.tryEntries[i];

                        if (entry.tryLoc === tryLoc) {
                            var record = entry.completion;

                            if (record.type === "throw") {
                                var thrown = record.arg;
                                resetTryEntry(entry);
                            }

                            return thrown;
                        }
                    } // The context.catch method must only be called with a location
                    // argument that corresponds to a known catch block.


                    throw new Error("illegal catch attempt");
                },
                delegateYield: function (iterable, resultName, nextLoc) {
                    this.delegate = {
                        iterator: values(iterable),
                        resultName: resultName,
                        nextLoc: nextLoc
                    };

                    if (this.method === "next") {
                        // Deliberately forget the last sent value so that we don't
                        // accidentally pass it on to the delegate.
                        this.arg = undefined$1;
                    }

                    return ContinueSentinel;
                }
            }; // Regardless of whether this script is executing as a CommonJS module
            // or not, return the runtime object so that we can declare the variable
            // regeneratorRuntime in the outer scope, which allows this module to be
            // injected easily by `bin/regenerator --include-runtime script.js`.

            return exports;
        }( // If this script is executing as a CommonJS module, use module.exports
            // as the regeneratorRuntime namespace. Otherwise create a new empty
            // object. Either way, the resulting object will be used to initialize
            // the regeneratorRuntime variable at the top of this file.
            module.exports );

        try {
            regeneratorRuntime = runtime;
        } catch (accidentalStrictMode) {
            // This module should not be running in strict mode, so the above
            // assignment should always work unless something is misconfigured. Just
            // in case runtime.js accidentally runs in strict mode, we can escape
            // strict mode using a global Function call. This could conceivably fail
            // if a Content Security Policy forbids using Function, but in that case
            // the proper solution is to fix the accidental strict mode problem. If
            // you've misconfigured your bundler to force strict mode and applied a
            // CSP to forbid Function, and you're not willing to fix either of those
            // problems, please detail your unique predicament in a GitHub issue.
            Function("r", "regeneratorRuntime = r")(runtime);
        }
    });

    var LHBaseClass = /*#__PURE__*/function () {
        function LHBaseClass(params) {
            _classCallCheck(this, LHBaseClass);
        }

        _createClass(LHBaseClass, [{
            key: "getParam",
            value: function getParam(params, strKey, defaultValue) {
                params = params || {};

                if (strKey in params) {
                    return params[strKey];
                } else if (defaultValue === undefined) {
                    this.throwException(strKey + " is a required parameter", "Parameters Error");
                } else {
                    return defaultValue;
                }
            }
        }, {
            key: "throwException",
            value: function throwException(message) {
                var title = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : "Error";
                throw new Error(this.constructor.name + " -- " + title + ": " + message);
            }
        }]);

        return LHBaseClass;
    }();

    var LHBaseClass_1 = LHBaseClass;

    var LHDelegate = /*#__PURE__*/function (_LHBaseClass) {
        _inherits(LHDelegate, _LHBaseClass);

        var _super = _createSuper(LHDelegate);

        function LHDelegate(params) {
            var _this;

            _classCallCheck(this, LHDelegate);

            _this = _super.call(this, params);
            _this.delegate = _this.getParam(params, "delegate", null);
            _this.delegateTypes = [];
            return _this;
        }

        _createClass(LHDelegate, [{
            key: "notify",
            value: function () {
                var _notify = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee(delegateString) {
                    var object,
                        _args = arguments;
                    return regeneratorRuntime.wrap(function _callee$(_context) {
                        while (1) {
                            switch (_context.prev = _context.next) {
                                case 0:
                                    object = _args.length > 1 && _args[1] !== undefined ? _args[1] : null;

                                    if (!this.delegateTypes.includes(delegateString)) {
                                        this.throwException("delegateString:" + delegateString + " is not defined in delegateTypes");
                                    }

                                    if (this.delegate) {
                                        this.delegate.receive(this, delegateString, object);
                                    }

                                case 3:
                                case "end":
                                    return _context.stop();
                            }
                        }
                    }, _callee, this);
                }));

                function notify(_x) {
                    return _notify.apply(this, arguments);
                }

                return notify;
            }()
        }, {
            key: "receive",
            value: function () {
                var _receive = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee2(notifier, delegateString) {
                    return regeneratorRuntime.wrap(function _callee2$(_context2) {
                        while (1) {
                            switch (_context2.prev = _context2.next) {
                                case 0:

                                case 1:
                                case "end":
                                    return _context2.stop();
                            }
                        }
                    }, _callee2);
                }));

                function receive(_x2, _x3) {
                    return _receive.apply(this, arguments);
                }

                return receive;
            }()
        }]);

        return LHDelegate;
    }(LHBaseClass_1);

    var LHDelegate_1 = LHDelegate;

    var propertyTypes = {
        STRING: "string",
        BOOL: "boolean",
        DATETIME: "dateTime",
        FILE: "attachment",
        NUMBER: "number",
        DECIMAL: "decimal",
        DATE: "extendedDateTime",
        // GUID: "guid",
        // AUTOGUID: "guid",
        // HYPERLINK: "object",
        // IMAGE: "image",
        MEMO: "extendedString" // MULTIVALUE: "object",
        // TIME: "extendedDateTime",
        // AUTONUMBER: "extendedNumber",
        // XML: "extendedString"

    };
    var methodTypes = {
        LIST: "list",
        READ: "read",
        CREATE: "create",
        EXECUTE: "execute",
        UPDATE: "update",
        DELETE: "delete"
    };
    var propertyTypes_1 = propertyTypes;
    var methodTypes_1 = methodTypes;
    var k2Types = {
        propertyTypes: propertyTypes_1,
        methodTypes: methodTypes_1
    };

    var propertyTypes$1 = k2Types.propertyTypes,
        methodTypes$1 = k2Types.methodTypes;

    var K2Base = /*#__PURE__*/function (_LHDelegate) {
        _inherits(K2Base, _LHDelegate);

        var _super = _createSuper(K2Base);

        function K2Base(params) {
            var _this;

            _classCallCheck(this, K2Base);

            _this = _super.call(this, params);
            _this.propertyTypes = _objectSpread2({}, propertyTypes$1);
            _this.methodTypes = _objectSpread2({}, methodTypes$1);
            return _this;
        }

        return K2Base;
    }(LHDelegate_1);

    var K2Base_1 = K2Base;

    var K2BaseIntegration = /*#__PURE__*/function (_K2Base) {
        _inherits(K2BaseIntegration, _K2Base);

        var _super = _createSuper(K2BaseIntegration);

        function K2BaseIntegration(params) {
            var _this;

            _classCallCheck(this, K2BaseIntegration);

            _this = _super.call(this, params);
            _this.metaData = {
                systemName: null,
                displayName: null,
                description: null
            };
            _this.smartObjects = [];
            return _this;
        }

        _createClass(K2BaseIntegration, [{
            key: "getSmartObject",
            value: function getSmartObject(name) {
                var _iterator = _createForOfIteratorHelper(this.smartObjects),
                    _step;

                try {
                    for (_iterator.s(); !(_step = _iterator.n()).done;) {
                        var obj = _step.value;

                        if (obj.name === name) {
                            return obj;
                        }
                    }
                } catch (err) {
                    _iterator.e(err);
                } finally {
                    _iterator.f();
                }

                this.throwException("Smart Object does not exist!");
            }
        }, {
            key: "getMetaData",
            value: function getMetaData() {
                return this.metaData;
            }
        }, {
            key: "getSchemas",
            value: function getSchemas() {
                var returnSchema = {};

                var _iterator2 = _createForOfIteratorHelper(this.smartObjects),
                    _step2;

                try {
                    for (_iterator2.s(); !(_step2 = _iterator2.n()).done;) {
                        var obj = _step2.value;
                        returnSchema[obj.name] = obj.getSchema();
                    }
                } catch (err) {
                    _iterator2.e(err);
                } finally {
                    _iterator2.f();
                }

                return {
                    displayName: this.metaData.displayName,
                    description: this.metaData.description,
                    objects: returnSchema
                };
            }
        }, {
            key: "execute",
            value: function () {
                var _execute = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee(objectName, methodName, parameters, properties) {
                    var obj;
                    return regeneratorRuntime.wrap(function _callee$(_context) {
                        while (1) {
                            switch (_context.prev = _context.next) {
                                case 0:
                                    obj = this.getSmartObject(objectName);
                                    _context.next = 3;
                                    return obj[methodName](parameters, properties);

                                case 3:
                                    return _context.abrupt("return", _context.sent);

                                case 4:
                                case "end":
                                    return _context.stop();
                            }
                        }
                    }, _callee, this);
                }));

                function execute(_x, _x2, _x3, _x4) {
                    return _execute.apply(this, arguments);
                }

                return execute;
            }()
        }]);

        return K2BaseIntegration;
    }(K2Base_1);

    var K2BaseIntegration_1 = K2BaseIntegration;

    var K2BaseSmartObject = /*#__PURE__*/function (_K2Base) {
        _inherits(K2BaseSmartObject, _K2Base);

        var _super = _createSuper(K2BaseSmartObject);

        function K2BaseSmartObject(params) {
            var _this;

            _classCallCheck(this, K2BaseSmartObject);

            _this = _super.call(this, params);
            _this.name = "K2BaseSmartObject";
            _this.displayName = "K2 BaseSmart Object";
            _this.description = "K2 BaseSmart Object";
            _this.api = _this.getParam(params, "api");
            _this.props = {};
            return _this;
        }

        _createClass(K2BaseSmartObject, [{
            key: "getProperties",
            value: function getProperties() {
                return {};
            }
        }, {
            key: "getMethods",
            value: function getMethods() {
                return {};
            }
        }, {
            key: "getSchema",
            value: function getSchema() {
                return {
                    displayName: this.displayName,
                    description: this.description,
                    properties: this.getProperties(),
                    methods: this.getMethods()
                };
            }
        }]);

        return K2BaseSmartObject;
    }(K2Base_1);

    var K2BaseSmartObject_1 = K2BaseSmartObject;

    var propertyTypes$2 = k2Types.propertyTypes,
        methodTypes$2 = k2Types.methodTypes;
    var fileThings = {
        fileProps: {
            id: "id",
            name: "name",
            path: "path",
            shareUrl: "shareUrl",
            size: "size",
            sourcePath: "sourcePath",
            destinationPath: "destinationPath",
            modifiedDate: "modifiedDate",
            directory: "directory",
            tags: "tags",
            parentFolderId: "parentFolderId",
            file: "File",
            // properties: "properties",
            tagName: "tagName",
            tagValue: "tagValue",
            result: "result"
        },

        get filePropertiesObj() {
            var _ref;

            return _ref = {}, _defineProperty(_ref, this.fileProps.id, {
                displayName: "File Id",
                description: "File Id",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.name, {
                displayName: "File Name",
                description: "File Name",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.path, {
                displayName: "Path",
                description: "Path",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.shareUrl, {
                displayName: "Share URL",
                description: "Share URL",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.file, {
                displayName: "File",
                description: "Input File Prop",
                type: propertyTypes$2.FILE
            }), _defineProperty(_ref, this.fileProps.size, {
                displayName: "File Size",
                description: "Size",
                type: propertyTypes$2.NUMBER
            }), _defineProperty(_ref, this.fileProps.sourcePath, {
                displayName: "Source Path",
                description: "Source Path",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.destinationPath, {
                displayName: "Destination Path",
                description: "Destination Path",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.modifiedDate, {
                displayName: "Modified Date",
                description: "Modified Date",
                type: propertyTypes$2.DATETIME
            }), _defineProperty(_ref, this.fileProps.directory, {
                displayName: "Directory",
                description: "Directory",
                type: propertyTypes$2.BOOL
            }), _defineProperty(_ref, this.fileProps.parentFolderId, {
                displayName: "Parent Folder ID",
                description: "Parent Folder ID",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.tags, {
                displayName: "Tags",
                description: "Tags",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.tagName, {
                displayName: "Tag Name",
                description: "Tag Name",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.tagValue, {
                displayName: "Tag Value",
                description: "Tag Value",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref, this.fileProps.result, {
                displayName: "File Upload Results",
                description: "File Upload Results",
                type: propertyTypes$2.STRING
            }), _ref;
        },

        fileMethods: {
            getInfo: "getInfo",
            getInfoById: "getInfoById",
            getShareUrl: "getShareUrl",
            getShareUrlById: "getShareUrlById",
            download: "download",
            copy: "copy",
            "delete": "delete",
            move: "move",
            upload: "upload",
            updateTags: "updateTags",
            updateSingleTag: "updateSingleTag"
        },

        get fileMethodsObj() {
            var _ref2;

            return _ref2 = {}, _defineProperty(_ref2, this.fileMethods.getInfo, {
                displayName: "Get Info",
                description: "Get info for the file by a given path.",
                type: methodTypes$2.READ,
                inputs: [this.fileProps.path],
                requiredInputs: [this.fileProps.path],
                outputs: [this.fileProps.id, this.fileProps.name, this.fileProps.parentFolderId, this.fileProps.directory, // this.fileProps.properties,
                    this.fileProps.tags, this.fileProps.path, this.fileProps.size, this.fileProps.modifiedDate]
            }), _defineProperty(_ref2, this.fileMethods.getInfoById, {
                displayName: "Get Info From Id",
                description: "Get metadata for a given file.",
                type: methodTypes$2.READ,
                inputs: [this.fileProps.id],
                requiredInputs: [this.fileProps.id],
                outputs: [this.fileProps.id, this.fileProps.name, this.fileProps.parentFolderId, this.fileProps.directory, // this.fileProps.properties,
                    this.fileProps.tags, this.fileProps.path, this.fileProps.size, this.fileProps.modifiedDate]
            }), _defineProperty(_ref2, this.fileMethods.getShareUrl, {
                displayName: "Get Folder Share URL",
                description: "Gets a basic share URL for a folder.",
                type: methodTypes$2.CREATE,
                inputs: [this.fileProps.path],
                requiredInputs: [this.fileProps.path],
                outputs: [this.fileProps.shareUrl]
            }), _defineProperty(_ref2, this.fileMethods.getShareUrlById, {
                displayName: "Get Folder Share URL by Id",
                description: "Gets a basic share URL for a folder with an Id.",
                type: methodTypes$2.CREATE,
                inputs: [this.fileProps.id],
                requiredInputs: [this.fileProps.id],
                outputs: [this.fileProps.shareUrl]
            }), _defineProperty(_ref2, this.fileMethods.download, {
                displayName: "Download",
                type: methodTypes$2.READ,
                inputs: [this.fileProps.path],
                requiredInputs: [this.fileProps.path],
                outputs: [this.fileProps.id, this.fileProps.name, this.fileProps.parentFolderId, this.fileProps.directory, // this.fileProps.properties,
                    this.fileProps.tags, this.fileProps.path, this.fileProps.size, this.fileProps.modifiedDate, this.fileProps.file]
            }), _defineProperty(_ref2, this.fileMethods.copy, {
                displayName: "Copy File",
                description: "Copy a file into a given folder.",
                inputs: [this.fileProps.sourcePath, this.fileProps.destinationPath],
                requiredInputs: [this.fileProps.sourcePath, this.fileProps.destinationPath],
                type: methodTypes$2.CREATE,
                outputs: [this.fileProps.id, this.fileProps.name, this.fileProps.parentFolderId, this.fileProps.directory, // this.fileProps.properties,
                    this.fileProps.tags, this.fileProps.path, this.fileProps.size, this.fileProps.modifiedDate]
            }), _defineProperty(_ref2, this.fileMethods["delete"], {
                displayName: "Delete File",
                description: "Delete File",
                type: methodTypes$2.DELETE,
                inputs: [this.fileProps.path],
                requiredInputs: [this.fileProps.path],
                outputs: []
            }), _defineProperty(_ref2, this.fileMethods.move, {
                displayName: "Move File",
                description: "Move File",
                type: methodTypes$2.EXECUTE,
                inputs: [this.fileProps.sourcePath, this.fileProps.destinationPath],
                requiredInputs: [this.fileProps.sourcePath, this.fileProps.destinationPath],
                outputs: [this.fileProps.id, this.fileProps.name, this.fileProps.parentFolderId, this.fileProps.directory, // this.fileProps.properties,
                    this.fileProps.tags, this.fileProps.path, this.fileProps.size, this.fileProps.modifiedDate]
            }), _defineProperty(_ref2, this.fileMethods.upload, {
                displayName: "Upload File",
                description: "Upload a File",
                type: methodTypes$2.CREATE,
                inputs: [this.fileProps.path, this.fileProps.file],
                requiredInputs: [this.fileProps.path, this.fileProps.file],
                outputs: [this.fileProps.id, this.fileProps.name, // this.fileProps.parentFolderId,
                    // this.fileProps.directory,
                    // // this.fileProps.properties,
                    // this.fileProps.tags,
                    this.fileProps.path, // this.fileProps.size,
                    // this.fileProps.modifiedDate
                    this.fileProps.result]
            }), _defineProperty(_ref2, this.fileMethods.updateTags, {
                displayName: "Update Tags",
                description: "Update tags for a given file.",
                inputs: [this.fileProps.path, this.fileProps.tags],
                requiredInputs: [this.fileProps.path, this.fileProps.tags],
                type: methodTypes$2.UPDATE,
                outputs: [this.fileProps.id, this.fileProps.name, this.fileProps.parentFolderId, this.fileProps.directory, // this.fileProps.properties,
                    this.fileProps.tags, this.fileProps.path, this.fileProps.size, this.fileProps.modifiedDate]
            }), _defineProperty(_ref2, this.fileMethods.updateSingleTag, {
                displayName: "Update Single File Tag",
                description: "Update an individual metadata Tag of a File",
                // Success or no success
                type: methodTypes$2.UPDATE,
                inputs: [this.fileProps.path, this.fileProps.tagName, this.fileProps.tagValue],
                requiredInputs: [this.fileProps.path, this.fileProps.tagName, this.fileProps.tagValue],
                outputs: [this.fileProps.id, this.fileProps.name, this.fileProps.parentFolderId, this.fileProps.directory, // this.fileProps.properties,
                    this.fileProps.tags, this.fileProps.path, this.fileProps.size, this.fileProps.modifiedDate]
            }), _ref2;
        }

    };
    var folderThings = {
        folderProps: {
            id: "id",
            name: "name",
            path: "path",
            shareUrl: "shareUrl",
            size: "size",
            sourcePath: "sourcePath",
            destinationPath: "destinationPath",
            modifiedDate: "modifiedDate",
            directory: "directory",
            tags: "tags",
            parentFolderId: "parentFolderId",
            // properties: "properties",
            tagName: "tagName",
            tagValue: "tagValue"
        },

        get folderPropertiesObj() {
            var _ref3;

            return _ref3 = {}, _defineProperty(_ref3, this.folderProps.id, {
                displayName: "Folder Id",
                description: "Folder Id",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.name, {
                displayName: "Folder Name",
                description: "Folder Name",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.path, {
                displayName: "Path",
                description: "Path",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.shareUrl, {
                displayName: "Share URL",
                description: "Share URL",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.size, {
                displayName: "Size",
                description: "Size",
                type: propertyTypes$2.NUMBER
            }), _defineProperty(_ref3, this.folderProps.sourcePath, {
                displayName: "Source Path",
                description: "Source Path",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.destinationPath, {
                displayName: "Destination Path",
                description: "Destination Path",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.modifiedDate, {
                displayName: "Modified Date",
                description: "Modified Date",
                type: propertyTypes$2.DATETIME
            }), _defineProperty(_ref3, this.folderProps.directory, {
                displayName: "Directory",
                description: "Directory",
                type: propertyTypes$2.BOOL
            }), _defineProperty(_ref3, this.folderProps.tags, {
                displayName: "Tags",
                description: "Tags",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.parentFolderId, {
                displayName: "Parent Folder ID",
                description: "Parent Folder ID",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.tagName, {
                displayName: "Tag Name",
                description: "Tag Name",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref3, this.folderProps.tagValue, {
                displayName: "Tag Value",
                description: "Tag Value",
                type: propertyTypes$2.STRING
            }), _ref3;
        },

        folderMethods: {
            listContents: "listContents",
            getInfoById: "getInfoById",
            getInfo: "getInfo",
            copy: "copy",
            create: "create",
            "delete": "delete",
            getShareUrl: "getShareUrl",
            getShareUrlById: 'getShareUrlById',
            move: "move",
            updateTags: "updateTags",
            updateSingleTag: "updateSingleTag"
        },

        get folderMethodsObj() {
            var _ref4;

            return _ref4 = {}, _defineProperty(_ref4, this.folderMethods.listContents, {
                displayName: "List Contents",
                description: "List all contents in a given folder",
                type: methodTypes$2.LIST,
                inputs: [this.folderProps.path],
                requiredInputs: [this.folderProps.path],
                outputs: [this.folderProps.id, this.folderProps.directory, // this.folderProps.properties,
                    this.folderProps.tags, this.folderProps.path, this.folderProps.size, this.folderProps.parentFolderId, this.folderProps.name, this.folderProps.modifiedDate]
            }), _defineProperty(_ref4, this.folderMethods.getInfoById, {
                displayName: "Get Info From Id",
                description: "Get metadata for a given folder.",
                type: methodTypes$2.READ,
                inputs: [this.folderProps.id],
                requiredInputs: [this.folderProps.id],
                // add metadata to outputs
                outputs: [this.folderProps.id, this.folderProps.name, this.folderProps.path, this.folderProps.size, this.folderProps.modifiedDate, this.folderProps.parentFolderId, // this.folderProps.properties,
                    this.folderProps.tags, this.folderProps.directory]
            }), _defineProperty(_ref4, this.folderMethods.getInfo, {
                displayName: "Get Info From Path",
                description: "Get metadata for a given folder.",
                type: methodTypes$2.READ,
                inputs: [this.folderProps.path],
                requiredInputs: [this.folderProps.path],
                // add metadata to outputs
                outputs: [this.folderProps.id, this.folderProps.name, this.folderProps.path, this.folderProps.size, this.folderProps.modifiedDate, this.folderProps.parentFolderId, // this.folderProps.properties,
                    this.folderProps.tags, this.folderProps.directory]
            }), _defineProperty(_ref4, this.folderMethods.copy, {
                displayName: "Copy Folder",
                description: "Creates a copy of a folder, including its files.",
                type: methodTypes$2.CREATE,
                inputs: [this.folderProps.sourcePath, this.folderProps.destinationPath],
                requiredInputs: [this.folderProps.sourcePath, this.folderProps.destinationPath],
                outputs: [this.folderProps.id, this.folderProps.name, this.folderProps.parentFolderId, this.folderProps.directory, // this.folderProps.properties,
                    this.folderProps.tags, this.folderProps.path, this.folderProps.size, this.folderProps.modifiedDate]
            }), _defineProperty(_ref4, this.folderMethods.create, {
                displayName: "Create Folder",
                description: "Create a new folder given a path.",
                type: methodTypes$2.CREATE,
                inputs: [this.folderProps.path],
                requiredInputs: [this.folderProps.path],
                outputs: [this.folderProps.name, this.folderProps.id, this.folderProps.parentFolderId, this.folderProps.directory, // this.folderProps.properties,
                    this.folderProps.tags, this.folderProps.path, this.folderProps.size, this.folderProps.modifiedDate]
            }), _defineProperty(_ref4, this.folderMethods["delete"], {
                displayName: "Delete Folder",
                description: "Deletes a folder",
                type: methodTypes$2.DELETE,
                inputs: [this.folderProps.path],
                requiredInputs: [this.folderProps.path],
                outputs: []
            }), _defineProperty(_ref4, this.folderMethods.getShareUrl, {
                displayName: "Get Folder Share URL",
                description: "Gets a basic share URL for a folder.",
                type: methodTypes$2.CREATE,
                inputs: [this.folderProps.path],
                requiredInputs: [this.folderProps.path],
                outputs: [this.folderProps.shareUrl]
            }), _defineProperty(_ref4, this.folderMethods.getShareUrlById, {
                displayName: "Get Folder Share URL by Id",
                description: "Gets a basic share URL for a folder with an Id.",
                type: methodTypes$2.CREATE,
                inputs: [this.folderProps.id],
                requiredInputs: [this.folderProps.id],
                outputs: [this.folderProps.shareUrl]
            }), _defineProperty(_ref4, this.folderMethods.move, {
                displayName: "Move Folder",
                description: "Moves a folder to a new parent folder.",
                // Success or no success
                type: methodTypes$2.UPDATE,
                inputs: [this.folderProps.sourcePath, this.folderProps.destinationPath],
                requiredInputs: [this.folderProps.sourcePath, this.folderProps.destinationPath],
                outputs: [this.folderProps.id, this.folderProps.name, this.folderProps.parentFolderId, this.folderProps.directory, // this.folderProps.properties,
                    this.folderProps.tags, this.folderProps.path, this.folderProps.size, this.folderProps.modifiedDate]
            }), _defineProperty(_ref4, this.folderMethods.updateTags, {
                displayName: "Update Folder Tags",
                description: "Update the Tags of a Folder",
                // Success or no success
                type: methodTypes$2.UPDATE,
                inputs: [this.folderProps.path, this.folderProps.tags],
                requiredInputs: [this.folderProps.path, this.folderProps.tags],
                outputs: [this.folderProps.id, this.folderProps.name, this.folderProps.parentFolderId, this.folderProps.directory, // this.folderProps.properties,
                    this.folderProps.tags, this.folderProps.path, this.folderProps.size, this.folderProps.modifiedDate]
            }), _defineProperty(_ref4, this.folderMethods.updateSingleTag, {
                displayName: "Update Single Folder Tag",
                description: "Update an individual metadata Tag of a Folder",
                // Success or no success
                type: methodTypes$2.UPDATE,
                inputs: [this.folderProps.path, this.folderProps.tagName, this.folderProps.tagValue],
                requiredInputs: [this.folderProps.path, this.folderProps.tagName, this.folderProps.tagValue],
                outputs: [this.folderProps.id, this.folderProps.name, this.folderProps.parentFolderId, this.folderProps.directory, // this.folderProps.properties,
                    this.folderProps.tags, this.folderProps.path, this.folderProps.size, this.folderProps.modifiedDate]
            }), _ref4;
        }

    };
    var serviceThings = {
        serviceProps: {
            id: "id",
            name: "name",
            directory: "directory",
            // properties: "properties",
            tags: "tags",
            path: "path",
            size: "size",
            parentFolderId: "parentFolderId",
            modifiedDate: "modifiedDate",
            used: "used",
            shared: "shared",
            total: "total",
            keyWords: "keyWords"
        },

        get servicePropertiesObj() {
            var _ref5;

            return _ref5 = {}, _defineProperty(_ref5, this.serviceProps.id, {
                displayName: "Id",
                description: "Id",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref5, this.serviceProps.name, {
                displayName: "Name",
                description: "Name",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref5, this.serviceProps.directory, {
                displayName: "Directory",
                description: "Directory",
                type: propertyTypes$2.BOOL
            }), _defineProperty(_ref5, this.serviceProps.tags, {
                displayName: "Tags",
                description: "Tags",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref5, this.serviceProps.path, {
                displayName: "Path",
                description: "Path",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref5, this.serviceProps.size, {
                displayName: "Size",
                description: "size",
                type: propertyTypes$2.NUMBER
            }), _defineProperty(_ref5, this.serviceProps.parentFolderId, {
                displayName: "Parent Folder ID",
                description: "Parent Folder ID",
                type: propertyTypes$2.STRING
            }), _defineProperty(_ref5, this.serviceProps.modifiedDate, {
                displayName: "Modified Date",
                description: "Modified Date",
                type: propertyTypes$2.DATETIME
            }), _defineProperty(_ref5, this.serviceProps.used, {
                displayName: "Used",
                description: "Used",
                type: propertyTypes$2.NUMBER
            }), _defineProperty(_ref5, this.serviceProps.shared, {
                displayName: "Shared",
                description: "Shared",
                type: propertyTypes$2.NUMBER
            }), _defineProperty(_ref5, this.serviceProps.total, {
                displayName: "Total",
                description: "Total",
                type: propertyTypes$2.NUMBER
            }), _defineProperty(_ref5, this.serviceProps.keyWords, {
                displayName: "Search Query",
                description: "Search query string according to the service",
                type: propertyTypes$2.STRING
            }), _ref5;
        },

        serviceMethods: {
            search: "search",
            getQuota: "getQuota"
        },

        get serviceMethodsObj() {
            var _ref6;

            return _ref6 = {}, _defineProperty(_ref6, this.serviceMethods.search, {
                displayName: "Search",
                description: "Search for items",
                type: methodTypes$2.LIST,
                inputs: [this.serviceProps.keyWords],
                requiredInputs: [this.serviceProps.keyWords],
                outputs: [this.serviceProps.id, this.serviceProps.name, this.serviceProps.directory, this.serviceProps.path, this.serviceProps.parentFolderId, // this.serviceProps.properties,
                    this.serviceProps.tags, this.serviceProps.size, this.serviceProps.modifiedDate]
            }), _defineProperty(_ref6, this.serviceMethods.getQuota, {
                displayName: "Get Quota",
                description: "Get storage quota",
                inputs: [],
                requiredInputs: [],
                type: methodTypes$2.READ,
                outputs: [this.serviceProps.total, this.serviceProps.used, this.serviceProps.shared]
            }), _ref6;
        }

    };

    var fileStorageSharedPropertiesAndMethods = _objectSpread2({}, fileThings, {}, folderThings, {}, serviceThings);

    var fileProps = fileStorageSharedPropertiesAndMethods.fileProps,
        filePropertiesObj = fileStorageSharedPropertiesAndMethods.filePropertiesObj,
        fileMethods = fileStorageSharedPropertiesAndMethods.fileMethods,
        fileMethodsObj = fileStorageSharedPropertiesAndMethods.fileMethodsObj; // Remove Tag reference for Microsoft since this is impossible ATM
    // delete fileProps.tags;
    // delete fileProps.tagName;
    // delete fileProps.tagValue;
    // delete filePropertiesObj.tags;
    // delete filePropertiesObj.tagName;
    // delete filePropertiesObj.tagValue;

    delete fileMethods.updateTags;
    delete fileMethods.updateSingleTag;
    delete fileMethodsObj.updateTags;
    delete fileMethodsObj.updateSingleTag;

    var File = /*#__PURE__*/function (_K2BaseSmartObject) {
        _inherits(File, _K2BaseSmartObject);

        var _super = _createSuper(File);

        function File(params) {
            var _this;

            _classCallCheck(this, File);

            _this = _super.call(this, params);
            _this.name = "file";
            _this.displayName = "File";
            _this.description = "File";
            _this.props = _objectSpread2({}, fileProps);
            _this.methods = _objectSpread2({}, fileMethods);
            return _this;
        }

        _createClass(File, [{
            key: "getProperties",
            value: function getProperties() {
                return _objectSpread2({}, filePropertiesObj);
            }
        }, {
            key: "getMethods",
            value: function getMethods() {
                return _objectSpread2({}, fileMethodsObj);
            }
        }, {
            key: "getInfo",
            value: function () {
                var _getInfo = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee(params, properties) {
                    var _postResult;

                    var path, data;
                    return regeneratorRuntime.wrap(function _callee$(_context) {
                        while (1) {
                            switch (_context.prev = _context.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path);
                                    _context.next = 3;
                                    return this.api.getInfo(path);

                                case 3:
                                    data = _context.sent;

                                    // let string = JSON.stringify(data);
                                    if (data.folder) {
                                        this.throwException("Attempting to retrieve info for a Folder. Please provide a valid file path.");
                                    }

                                    postResult((_postResult = {}, _defineProperty(_postResult, this.props.id, data.id), _defineProperty(_postResult, this.props.name, data.name), _defineProperty(_postResult, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult, this.props.directory, data.folder ? true : false), _defineProperty(_postResult, this.props.tags, ''), _defineProperty(_postResult, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult, this.props.size, data.size), _defineProperty(_postResult, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult));

                                case 6:
                                case "end":
                                    return _context.stop();
                            }
                        }
                    }, _callee, this);
                }));

                function getInfo(_x, _x2) {
                    return _getInfo.apply(this, arguments);
                }

                return getInfo;
            }()
        }, {
            key: "getInfoById",
            value: function () {
                var _getInfoById = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee2(params, properties) {
                    var _postResult2;

                    var id, data, string;
                    return regeneratorRuntime.wrap(function _callee2$(_context2) {
                        while (1) {
                            switch (_context2.prev = _context2.next) {
                                case 0:
                                    id = this.getParam(properties, this.props.id);
                                    _context2.next = 3;
                                    return this.api.getInfoById(id);

                                case 3:
                                    data = _context2.sent;
                                    string = JSON.stringify(data);
                                    postResult((_postResult2 = {}, _defineProperty(_postResult2, this.props.id, data.id), _defineProperty(_postResult2, this.props.name, data.name), _defineProperty(_postResult2, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult2, this.props.directory, data.folder ? true : false), _defineProperty(_postResult2, this.props.tags, ''), _defineProperty(_postResult2, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult2, this.props.size, data.size), _defineProperty(_postResult2, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult2));

                                case 6:
                                case "end":
                                    return _context2.stop();
                            }
                        }
                    }, _callee2, this);
                }));

                function getInfoById(_x3, _x4) {
                    return _getInfoById.apply(this, arguments);
                }

                return getInfoById;
            }() // get share url by path

        }, {
            key: "getShareUrl",
            value: function () {
                var _getShareUrl = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee3(params, properties) {
                    var path, data;
                    return regeneratorRuntime.wrap(function _callee3$(_context3) {
                        while (1) {
                            switch (_context3.prev = _context3.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path);
                                    _context3.next = 3;
                                    return this.api.getShareUrl(path);

                                case 3:
                                    data = _context3.sent;
                                    postResult(_defineProperty({}, this.props.shareUrl, data.link.webUrl));

                                case 5:
                                case "end":
                                    return _context3.stop();
                            }
                        }
                    }, _callee3, this);
                }));

                function getShareUrl(_x5, _x6) {
                    return _getShareUrl.apply(this, arguments);
                }

                return getShareUrl;
            }()
        }, {
            key: "getShareUrlById",
            value: function () {
                var _getShareUrlById = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee4(params, properties) {
                    var id, data;
                    return regeneratorRuntime.wrap(function _callee4$(_context4) {
                        while (1) {
                            switch (_context4.prev = _context4.next) {
                                case 0:
                                    id = this.getParam(properties, this.props.id);
                                    _context4.next = 3;
                                    return this.api.getShareUrlById(id);

                                case 3:
                                    data = _context4.sent;
                                    postResult(_defineProperty({}, this.props.shareUrl, data.link.webUrl));

                                case 5:
                                case "end":
                                    return _context4.stop();
                            }
                        }
                    }, _callee4, this);
                }));

                function getShareUrlById(_x7, _x8) {
                    return _getShareUrlById.apply(this, arguments);
                }

                return getShareUrlById;
            }() // TODO: Fix
            // DOC: https://docs.microsoft.com/en-us/graph/api/driveitem-get-content?view=graph-rest-1.0&tabs=http

        }, {
            key: "download",
            value: function () {
                var _download = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee5(params, properties) {
                    var path, item, downloadUrl, xhr;
                    return regeneratorRuntime.wrap(function _callee5$(_context5) {
                        while (1) {
                            switch (_context5.prev = _context5.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path); // Get file ID from the Path, and the File MimeType

                                    _context5.next = 3;
                                    return this.api.getInfo(path);

                                case 3:
                                    item = _context5.sent;
                                    // let mimeType = this.api.mimeTypeMapping(item.mimeType)
                                    downloadUrl = this.api.baseUrl + this.api.URLEndpoints.download(path); //TODO re-enable after resolving
                                    // let data = await this.api.downloadFile(item.id, item.mimeType);

                                    xhr = new XMLHttpRequest();
                                    xhr.withCredentials = true;

                                    xhr.onreadystatechange = function () {
                                        if (xhr.readyState !== 4) return;
                                        if (xhr.status !== 200) throw new Error("Request to download from ".concat(downloadUrl, " failed with status ").concat(xhr.status, " ").concat(xhr.statusText, " and response ").concat(JSON.stringify(xhr.response), ". Here's the whole xhr object: ").concat(JSON.stringify(xhr), " "));
                                        postResult({
                                            "id": item.id,
                                            "name": item.name,
                                            "parentFolderId": item.parentReference.id,
                                            "directory": item.folder ? true : false,
                                            // [this.props.properties]: JSON.stringify(data)
                                            "tags": '',
                                            "path": path,
                                            "size": item.size,
                                            "modifiedDate": new Date(item.lastModifiedDateTime),
                                            "File": {
                                                filename: item.name,
                                                content: xhr.response
                                            }
                                        });
                                    };

                                    xhr.open("GET", downloadUrl);
                                    xhr.setRequestHeader("Content-Type", "application/json");
                                    xhr.responseType = 'blob';
                                    _context5.next = 13;
                                    return xhr.send();

                                case 13:
                                case "end":
                                    return _context5.stop();
                            }
                        }
                    }, _callee5, this);
                }));

                function download(_x9, _x10) {
                    return _download.apply(this, arguments);
                }

                return download;
            }() // copies a file to a given path

        }, {
            key: "copy",
            value: function () {
                var _copy = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee6(params, properties) {
                    var _postResult5;

                    var sourcePath, destinationPath, data;
                    return regeneratorRuntime.wrap(function _callee6$(_context6) {
                        while (1) {
                            switch (_context6.prev = _context6.next) {
                                case 0:
                                    // Change
                                    sourcePath = this.getParam(properties, this.props.sourcePath);
                                    destinationPath = this.getParam(properties, this.props.destinationPath);
                                    _context6.next = 4;
                                    return this.api.copy(sourcePath, destinationPath);

                                case 4:
                                    data = _context6.sent;
                                    console.log(data);
                                    postResult((_postResult5 = {}, _defineProperty(_postResult5, this.props.id, data.id), _defineProperty(_postResult5, this.props.name, data.name), _defineProperty(_postResult5, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult5, this.props.tags, ''), _defineProperty(_postResult5, this.props.directory, data.folder ? true : false), _defineProperty(_postResult5, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult5, this.props.size, data.size), _defineProperty(_postResult5, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult5));

                                case 7:
                                case "end":
                                    return _context6.stop();
                            }
                        }
                    }, _callee6, this);
                }));

                function copy(_x11, _x12) {
                    return _copy.apply(this, arguments);
                }

                return copy;
            }()
        }, {
            key: "delete",
            value: function () {
                var _delete2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee7(params, properties) {
                    var path, res;
                    return regeneratorRuntime.wrap(function _callee7$(_context7) {
                        while (1) {
                            switch (_context7.prev = _context7.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path);
                                    _context7.next = 3;
                                    return this.api.deleteFileOrFolder(path);

                                case 3:
                                    res = _context7.sent;

                                    if (!(res == true)) {
                                        _context7.next = 6;
                                        break;
                                    }

                                    return _context7.abrupt("return", true);

                                case 6:
                                case "end":
                                    return _context7.stop();
                            }
                        }
                    }, _callee7, this);
                }));

                function _delete(_x13, _x14) {
                    return _delete2.apply(this, arguments);
                }

                return _delete;
            }()
        }, {
            key: "move",
            value: function () {
                var _move = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee8(params, properties) {
                    var _postResult6;

                    var sourcePath, destinationPath, data;
                    return regeneratorRuntime.wrap(function _callee8$(_context8) {
                        while (1) {
                            switch (_context8.prev = _context8.next) {
                                case 0:
                                    sourcePath = this.getParam(properties, this.props.sourcePath);
                                    destinationPath = this.getParam(properties, this.props.destinationPath);
                                    _context8.next = 4;
                                    return this.api.moveFileOrFolder(sourcePath, destinationPath);

                                case 4:
                                    data = _context8.sent;
                                    postResult((_postResult6 = {}, _defineProperty(_postResult6, this.props.id, data.id), _defineProperty(_postResult6, this.props.name, data.name), _defineProperty(_postResult6, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult6, this.props.tags, ''), _defineProperty(_postResult6, this.props.directory, data.folder ? true : false), _defineProperty(_postResult6, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult6, this.props.size, data.size), _defineProperty(_postResult6, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult6));

                                case 6:
                                case "end":
                                    return _context8.stop();
                            }
                        }
                    }, _callee8, this);
                }));

                function move(_x15, _x16) {
                    return _move.apply(this, arguments);
                }

                return move;
            }() //TODO need an Upload function

        }, {
            key: "upload",
            value: function () {
                var _upload = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee9(params, properties) {
                    return regeneratorRuntime.wrap(function _callee9$(_context9) {
                        while (1) {
                            switch (_context9.prev = _context9.next) {
                                case 0:
                                    return _context9.abrupt("return");

                                case 1:
                                case "end":
                                    return _context9.stop();
                            }
                        }
                    }, _callee9);
                }));

                function upload(_x17, _x18) {
                    return _upload.apply(this, arguments);
                }

                return upload;
            }() // //TODO need an UpdateTags function
            // async updateTags (params, properties) {
            //   return
            // }

        }]);

        return File;
    }(K2BaseSmartObject_1);

    var File_1 = File;

    var folderProps = fileStorageSharedPropertiesAndMethods.folderProps,
        folderPropertiesObj = fileStorageSharedPropertiesAndMethods.folderPropertiesObj,
        folderMethods = fileStorageSharedPropertiesAndMethods.folderMethods,
        folderMethodsObj = fileStorageSharedPropertiesAndMethods.folderMethodsObj; // Remove tagging related Methods and Props

    delete folderMethods.updateTags;
    delete folderMethods.updateSingleTag;
    delete folderMethodsObj.updateTags;
    delete folderMethodsObj.updateSingleTag;

    var Folder = /*#__PURE__*/function (_K2BaseSmartObject) {
        _inherits(Folder, _K2BaseSmartObject);

        var _super = _createSuper(Folder);

        function Folder(params) {
            var _this;

            _classCallCheck(this, Folder);

            _this = _super.call(this, params);
            _this.name = "folder";
            _this.displayName = "Folder";
            _this.description = "Folder";
            _this.props = _objectSpread2({}, folderProps);
            _this.methods = _objectSpread2({}, folderMethods);
            return _this;
        } // define all the properties that will be used by this smart object


        _createClass(Folder, [{
            key: "getProperties",
            value: function getProperties() {
                return _objectSpread2({}, folderPropertiesObj);
            } // define all the methods and their inputs / outputs for the smart object

        }, {
            key: "getMethods",
            value: function getMethods() {
                return _objectSpread2({}, folderMethodsObj);
            } // get the info for a folder

        }, {
            key: "getInfoById",
            value: function () {
                var _getInfoById = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee(params, properties) {
                    var _postResult;

                    var id, data;
                    return regeneratorRuntime.wrap(function _callee$(_context) {
                        while (1) {
                            switch (_context.prev = _context.next) {
                                case 0:
                                    id = this.getParam(properties, this.props.id);
                                    _context.next = 3;
                                    return this.api.getInfoById(id);

                                case 3:
                                    data = _context.sent;
                                    postResult((_postResult = {}, _defineProperty(_postResult, this.props.id, data.id), _defineProperty(_postResult, this.props.name, data.name), _defineProperty(_postResult, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult, this.props.tags, ''), _defineProperty(_postResult, this.props.directory, true), _defineProperty(_postResult, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult, this.props.size, "".concat(data.size)), _defineProperty(_postResult, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult));

                                case 5:
                                case "end":
                                    return _context.stop();
                            }
                        }
                    }, _callee, this);
                }));

                function getInfoById(_x, _x2) {
                    return _getInfoById.apply(this, arguments);
                }

                return getInfoById;
            }()
        }, {
            key: "getInfo",
            value: function () {
                var _getInfo = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee2(params, properties) {
                    var _postResult2;

                    var path, data;
                    return regeneratorRuntime.wrap(function _callee2$(_context2) {
                        while (1) {
                            switch (_context2.prev = _context2.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path);
                                    _context2.next = 3;
                                    return this.api.getInfo(path);

                                case 3:
                                    data = _context2.sent;
                                    postResult((_postResult2 = {}, _defineProperty(_postResult2, this.props.id, data.id), _defineProperty(_postResult2, this.props.name, data.name), _defineProperty(_postResult2, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult2, this.props.tags, ''), _defineProperty(_postResult2, this.props.directory, true), _defineProperty(_postResult2, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult2, this.props.size, "".concat(data.size)), _defineProperty(_postResult2, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult2));

                                case 5:
                                case "end":
                                    return _context2.stop();
                            }
                        }
                    }, _callee2, this);
                }));

                function getInfo(_x3, _x4) {
                    return _getInfo.apply(this, arguments);
                }

                return getInfo;
            }() // listContentss contents of a folder with given id (changed to path)

        }, {
            key: "listContents",
            value: function () {
                var _listContents = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee3(params, properties) {
                    var _this2 = this;

                    var path, res, results;
                    return regeneratorRuntime.wrap(function _callee3$(_context3) {
                        while (1) {
                            switch (_context3.prev = _context3.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path);
                                    _context3.next = 3;
                                    return this.api.listFolderContentsByPath(path);

                                case 3:
                                    res = _context3.sent;
                                    results = res.value;
                                    postResult(results.map(function (data) {
                                        var _ref;

                                        return _ref = {}, _defineProperty(_ref, _this2.props.id, data.id), _defineProperty(_ref, _this2.props.name, data.name), _defineProperty(_ref, _this2.props.directory, data.folder ? true : false), _defineProperty(_ref, _this2.props.parentFolderId, data.parentReference.id), _defineProperty(_ref, _this2.props.tags, ''), _defineProperty(_ref, _this2.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_ref, _this2.props.size, data.size), _defineProperty(_ref, _this2.props.modifiedDate, new Date(data.lastModifiedDateTime)), _ref;
                                    }));

                                case 6:
                                case "end":
                                    return _context3.stop();
                            }
                        }
                    }, _callee3, this);
                }));

                function listContents(_x5, _x6) {
                    return _listContents.apply(this, arguments);
                }

                return listContents;
            }()
        }, {
            key: "getShareUrl",
            value: function () {
                var _getShareUrl = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee4(params, properties) {
                    var path, data;
                    return regeneratorRuntime.wrap(function _callee4$(_context4) {
                        while (1) {
                            switch (_context4.prev = _context4.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path);
                                    _context4.next = 3;
                                    return this.api.getShareUrl(path);

                                case 3:
                                    data = _context4.sent;
                                    postResult(_defineProperty({}, this.props.shareUrl, data.link.webUrl));

                                case 5:
                                case "end":
                                    return _context4.stop();
                            }
                        }
                    }, _callee4, this);
                }));

                function getShareUrl(_x7, _x8) {
                    return _getShareUrl.apply(this, arguments);
                }

                return getShareUrl;
            }()
        }, {
            key: "getShareUrlById",
            value: function () {
                var _getShareUrlById = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee5(params, properties) {
                    var id, data;
                    return regeneratorRuntime.wrap(function _callee5$(_context5) {
                        while (1) {
                            switch (_context5.prev = _context5.next) {
                                case 0:
                                    id = this.getParam(properties, this.props.id);
                                    _context5.next = 3;
                                    return this.api.getShareUrlById(id);

                                case 3:
                                    data = _context5.sent;
                                    postResult(_defineProperty({}, this.props.shareUrl, data.link.webUrl));

                                case 5:
                                case "end":
                                    return _context5.stop();
                            }
                        }
                    }, _callee5, this);
                }));

                function getShareUrlById(_x9, _x10) {
                    return _getShareUrlById.apply(this, arguments);
                }

                return getShareUrlById;
            }() // https://docs.microsoft.com/en-us/graph/api/driveitem-copy?view=graph-rest-1.0&tabs=http

        }, {
            key: "copy",
            value: function () {
                var _copy = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee6(params, properties) {
                    var _postResult5;

                    var sourcePath, destinationPath, data;
                    return regeneratorRuntime.wrap(function _callee6$(_context6) {
                        while (1) {
                            switch (_context6.prev = _context6.next) {
                                case 0:
                                    sourcePath = this.getParam(properties, this.props.sourcePath);
                                    console.log(sourcePath);
                                    destinationPath = this.getParam(properties, this.props.destinationPath);

                                    if (sourcePath == destinationPath) {
                                        this.throwException("Cannot create a copy of a folder within itself.");
                                    }

                                    _context6.next = 6;
                                    return this.api.copy(sourcePath, destinationPath);

                                case 6:
                                    data = _context6.sent;
                                    console.log(data);
                                    postResult((_postResult5 = {}, _defineProperty(_postResult5, this.props.id, data.id), _defineProperty(_postResult5, this.props.name, data.name), _defineProperty(_postResult5, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult5, this.props.tags, ''), _defineProperty(_postResult5, this.props.directory, true), _defineProperty(_postResult5, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult5, this.props.size, data.size), _defineProperty(_postResult5, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult5));

                                case 9:
                                case "end":
                                    return _context6.stop();
                            }
                        }
                    }, _callee6, this);
                }));

                function copy(_x11, _x12) {
                    return _copy.apply(this, arguments);
                }

                return copy;
            }() // Creates a new folder by path

        }, {
            key: "create",
            value: function () {
                var _create = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee7(params, properties) {
                    var _postResult6;

                    var path, splitPath, name, parentPath, data;
                    return regeneratorRuntime.wrap(function _callee7$(_context7) {
                        while (1) {
                            switch (_context7.prev = _context7.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path);
                                    splitPath = path.split('/');
                                    name = splitPath[splitPath.length - 1];
                                    parentPath = splitPath.slice(0, splitPath.length - 1).join('/');

                                    if (!parentPath) {
                                        parentPath = '/';
                                    }

                                    _context7.next = 7;
                                    return this.api.createFolder(name, parentPath);

                                case 7:
                                    data = _context7.sent;
                                    // Add a '/' to parent reference's path for this new folder's path
                                    // const path = data.parentReference.path + "/";
                                    // If successful, returns `201 Created` and new folder info in body
                                    postResult((_postResult6 = {}, _defineProperty(_postResult6, this.props.id, data.id), _defineProperty(_postResult6, this.props.name, data.name), _defineProperty(_postResult6, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult6, this.props.tags, ''), _defineProperty(_postResult6, this.props.directory, true), _defineProperty(_postResult6, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult6, this.props.size, data.size), _defineProperty(_postResult6, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult6));

                                case 9:
                                case "end":
                                    return _context7.stop();
                            }
                        }
                    }, _callee7, this);
                }));

                function create(_x13, _x14) {
                    return _create.apply(this, arguments);
                }

                return create;
            }() // Deletes a folder by path

        }, {
            key: "delete",
            value: function () {
                var _delete2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee8(params, properties) {
                    var path, res;
                    return regeneratorRuntime.wrap(function _callee8$(_context8) {
                        while (1) {
                            switch (_context8.prev = _context8.next) {
                                case 0:
                                    path = this.getParam(properties, this.props.path);
                                    _context8.next = 3;
                                    return this.api.deleteFileOrFolder(path);

                                case 3:
                                    res = _context8.sent;

                                    if (!(res == true)) {
                                        _context8.next = 6;
                                        break;
                                    }

                                    return _context8.abrupt("return", true);

                                case 6:
                                case "end":
                                    return _context8.stop();
                            }
                        }
                    }, _callee8, this);
                }));

                function _delete(_x15, _x16) {
                    return _delete2.apply(this, arguments);
                }

                return _delete;
            }() //TODO Need a move function! sourcePath and destinationPath, remember

        }, {
            key: "move",
            value: function () {
                var _move = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee9(params, properties) {
                    var _postResult7;

                    var sourcePath, destinationPath, data;
                    return regeneratorRuntime.wrap(function _callee9$(_context9) {
                        while (1) {
                            switch (_context9.prev = _context9.next) {
                                case 0:
                                    sourcePath = this.getParam(properties, this.props.sourcePath);
                                    console.log(sourcePath);
                                    destinationPath = this.getParam(properties, this.props.destinationPath);

                                    if (sourcePath == destinationPath) {
                                        this.throwException("Cannot move a folder to itself.");
                                    }

                                    _context9.next = 6;
                                    return integration.api.moveFileOrFolder(sourcePath, destinationPath);

                                case 6:
                                    data = _context9.sent;
                                    postResult((_postResult7 = {}, _defineProperty(_postResult7, this.props.id, data.id), _defineProperty(_postResult7, this.props.name, data.name), _defineProperty(_postResult7, this.props.parentFolderId, data.parentReference.id), _defineProperty(_postResult7, this.props.tags, ''), _defineProperty(_postResult7, this.props.directory, data.folder ? true : false), _defineProperty(_postResult7, this.props.path, "".concat(data.parentReference.path, "/").concat(data.name)), _defineProperty(_postResult7, this.props.size, data.size), _defineProperty(_postResult7, this.props.modifiedDate, new Date(data.lastModifiedDateTime)), _postResult7));

                                case 8:
                                case "end":
                                    return _context9.stop();
                            }
                        }
                    }, _callee9, this);
                }));

                function move(_x17, _x18) {
                    return _move.apply(this, arguments);
                }

                return move;
            }()
        }, {
            key: "updateTags",
            value: function () {
                var _updateTags = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee10(params, properties) {
                    return regeneratorRuntime.wrap(function _callee10$(_context10) {
                        while (1) {
                            switch (_context10.prev = _context10.next) {
                                case 0:
                                    return _context10.abrupt("return");

                                case 1:
                                case "end":
                                    return _context10.stop();
                            }
                        }
                    }, _callee10);
                }));

                function updateTags(_x19, _x20) {
                    return _updateTags.apply(this, arguments);
                }

                return updateTags;
            }()
        }]);

        return Folder;
    }(K2BaseSmartObject_1);

    var Folder_1 = Folder;

    var serviceProps = fileStorageSharedPropertiesAndMethods.serviceProps,
        servicePropertiesObj = fileStorageSharedPropertiesAndMethods.servicePropertiesObj,
        serviceMethods = fileStorageSharedPropertiesAndMethods.serviceMethods,
        serviceMethodsObj = fileStorageSharedPropertiesAndMethods.serviceMethodsObj;
    delete serviceProps.shared;
    delete servicePropertiesObj.shared;
    serviceMethodsObj.getQuota.outputs = serviceMethodsObj.getQuota.outputs.filter(function (output) {
        return output !== 'shared';
    });

    var Service = /*#__PURE__*/function (_K2BaseSmartObject) {
        _inherits(Service, _K2BaseSmartObject);

        var _super = _createSuper(Service);

        function Service(params) {
            var _this;

            _classCallCheck(this, Service);

            _this = _super.call(this, params);
            _this.name = "service";
            _this.displayName = "Service";
            _this.description = "Service";
            _this.props = _objectSpread2({}, serviceProps);
            _this.methods = _objectSpread2({}, serviceMethods);
            return _this;
        }

        _createClass(Service, [{
            key: "getProperties",
            value: function getProperties() {
                return _objectSpread2({}, servicePropertiesObj);
            }
        }, {
            key: "getMethods",
            value: function getMethods() {
                return _objectSpread2({}, serviceMethodsObj);
            } //  Takes search string and returns items

        }, {
            key: "search",
            value: function () {
                var _search = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee(params, properties) {
                    var _this2 = this;

                    var searchString, res, data, batch, batchRes, dataWithPaths;
                    return regeneratorRuntime.wrap(function _callee$(_context) {
                        while (1) {
                            switch (_context.prev = _context.next) {
                                case 0:
                                    searchString = this.getParam(properties, this.props.keyWords);
                                    _context.next = 3;
                                    return this.api.searchDrive(searchString);

                                case 3:
                                    res = _context.sent;
                                    data = res.value;

                                    if (!(data.length > 0)) {
                                        _context.next = 14;
                                        break;
                                    }

                                    // Batch to save on potentially thousands of API requests... at least we can batch by 20
                                    batch = data.map(function (item) {
                                        var batchObj = {};
                                        batchObj.id = item.id;
                                        batchObj.method = 'GET';
                                        batchObj.url = "/me/drive/items/".concat(item.id, "?select=parentReference");
                                        return batchObj;
                                    });
                                    _context.next = 9;
                                    return this.api.batchRequest(batch);

                                case 9:
                                    batchRes = _context.sent;
                                    dataWithPaths = data.map(function (item) {
                                        var responseObject = batchRes.responses.find(function (response) {
                                            return response.id == item.id;
                                        });
                                        item.parentReference = responseObject.body.parentReference;
                                        return item;
                                    });
                                    return _context.abrupt("return", postResult(dataWithPaths.map(function (x) {
                                        var _ref;

                                        return _ref = {}, _defineProperty(_ref, _this2.props.id, x.id), _defineProperty(_ref, _this2.props.name, x.name), _defineProperty(_ref, _this2.props.directory, x.folder ? true : false), _defineProperty(_ref, _this2.props.path, "".concat(x.parentReference.path, "/").concat(x.name)), _defineProperty(_ref, _this2.props.parentFolderId, x.parentReference.id), _defineProperty(_ref, _this2.props.tags, ''), _defineProperty(_ref, _this2.props.size, x.size), _defineProperty(_ref, _this2.props.modifiedDate, new Date(x.lastModifiedDateTime)), _ref;
                                    })));

                                case 14:
                                    return _context.abrupt("return", postResult([]));

                                case 15:
                                case "end":
                                    return _context.stop();
                            }
                        }
                    }, _callee, this);
                }));

                function search(_x, _x2) {
                    return _search.apply(this, arguments);
                }

                return search;
            }()
        }, {
            key: "getQuota",
            value: function () {
                var _getQuota = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee2(params, properties) {
                    var _postResult;

                    var res, data;
                    return regeneratorRuntime.wrap(function _callee2$(_context2) {
                        while (1) {
                            switch (_context2.prev = _context2.next) {
                                case 0:
                                    _context2.next = 2;
                                    return this.api.getServiceQuota();

                                case 2:
                                    res = _context2.sent;
                                    console.log(res);
                                    data = res.quota; // Number/Integer _should_ work. ~Sean
                                    // let total = data.total.toString();
                                    // let used = data.used.toString();

                                    return _context2.abrupt("return", postResult((_postResult = {}, _defineProperty(_postResult, this.props.total, data.total), _defineProperty(_postResult, this.props.used, data.used), _postResult)));

                                case 6:
                                case "end":
                                    return _context2.stop();
                            }
                        }
                    }, _callee2, this);
                }));

                function getQuota(_x3, _x4) {
                    return _getQuota.apply(this, arguments);
                }

                return getQuota;
            }()
        }]);

        return Service;
    }(K2BaseSmartObject_1);

    var Service_1 = Service;

    var fetch = createCommonjsModule(function (module) {
        (function (self) {
            // with Ajax.

            if (!self.__disableNativeFetch && self.fetch) {
                return;
            }

            function normalizeName(name) {
                if (typeof name !== 'string') {
                    name = String(name);
                }

                if (/[^a-z0-9\-#$%&'*+.\^_`|~]/i.test(name)) {
                    throw new TypeError('Invalid character in header field name');
                }

                return name.toLowerCase();
            }

            function normalizeValue(value) {
                if (typeof value !== 'string') {
                    value = String(value);
                }

                return value;
            }

            function Headers(headers) {
                this.map = {};

                if (headers instanceof Headers) {
                    headers.forEach(function (value, name) {
                        this.append(name, value);
                    }, this);
                } else if (headers) {
                    Object.getOwnPropertyNames(headers).forEach(function (name) {
                        this.append(name, headers[name]);
                    }, this);
                }
            }

            Headers.prototype.append = function (name, value) {
                name = normalizeName(name);
                value = normalizeValue(value);
                var list = this.map[name];

                if (!list) {
                    list = [];
                    this.map[name] = list;
                }

                list.push(value);
            };

            Headers.prototype['delete'] = function (name) {
                delete this.map[normalizeName(name)];
            };

            Headers.prototype.get = function (name) {
                var values = this.map[normalizeName(name)];
                return values ? values[0] : null;
            };

            Headers.prototype.getAll = function (name) {
                return this.map[normalizeName(name)] || [];
            };

            Headers.prototype.has = function (name) {
                return this.map.hasOwnProperty(normalizeName(name));
            };

            Headers.prototype.set = function (name, value) {
                this.map[normalizeName(name)] = [normalizeValue(value)];
            };

            Headers.prototype.forEach = function (callback, thisArg) {
                Object.getOwnPropertyNames(this.map).forEach(function (name) {
                    this.map[name].forEach(function (value) {
                        callback.call(thisArg, value, name, this);
                    }, this);
                }, this);
            };

            function consumed(body) {
                if (body.bodyUsed) {
                    return Promise.reject(new TypeError('Already read'));
                }

                body.bodyUsed = true;
            }

            function fileReaderReady(reader) {
                return new Promise(function (resolve, reject) {
                    reader.onload = function () {
                        resolve(reader.result);
                    };

                    reader.onerror = function () {
                        reject(reader.error);
                    };
                });
            }

            function readBlobAsArrayBuffer(blob) {
                var reader = new FileReader();
                reader.readAsArrayBuffer(blob);
                return fileReaderReady(reader);
            }

            function readBlobAsText(blob, options) {
                var reader = new FileReader();
                var contentType = options.headers.map['content-type'] ? options.headers.map['content-type'].toString() : '';
                var regex = /charset\=[0-9a-zA-Z\-\_]*;?/;

                var _charset = blob.type.match(regex) || contentType.match(regex);

                var args = [blob];

                if (_charset) {
                    args.push(_charset[0].replace(/^charset\=/, '').replace(/;$/, ''));
                }

                reader.readAsText.apply(reader, args);
                return fileReaderReady(reader);
            }

            var support = {
                blob: 'FileReader' in self && 'Blob' in self && function () {
                    try {
                        new Blob();
                        return true;
                    } catch (e) {
                        return false;
                    }
                }(),
                formData: 'FormData' in self,
                arrayBuffer: 'ArrayBuffer' in self
            };

            function Body() {
                this.bodyUsed = false;

                this._initBody = function (body, options) {
                    this._bodyInit = body;

                    if (typeof body === 'string') {
                        this._bodyText = body;
                    } else if (support.blob && Blob.prototype.isPrototypeOf(body)) {
                        this._bodyBlob = body;
                        this._options = options;
                    } else if (support.formData && FormData.prototype.isPrototypeOf(body)) {
                        this._bodyFormData = body;
                    } else if (!body) {
                        this._bodyText = '';
                    } else if (support.arrayBuffer && ArrayBuffer.prototype.isPrototypeOf(body)) ;
                };

                if (support.blob) {
                    this.blob = function () {
                        var rejected = consumed(this);

                        if (rejected) {
                            return rejected;
                        }

                        if (this._bodyBlob) {
                            return Promise.resolve(this._bodyBlob);
                        } else if (this._bodyFormData) {
                            throw new Error('could not read FormData body as blob');
                        } else {
                            return Promise.resolve(new Blob([this._bodyText]));
                        }
                    };

                    this.arrayBuffer = function () {
                        return this.blob().then(readBlobAsArrayBuffer);
                    };

                    this.text = function () {
                        var rejected = consumed(this);

                        if (rejected) {
                            return rejected;
                        }

                        if (this._bodyBlob) {
                            return readBlobAsText(this._bodyBlob, this._options);
                        } else if (this._bodyFormData) {
                            throw new Error('could not read FormData body as text');
                        } else {
                            return Promise.resolve(this._bodyText);
                        }
                    };
                } else {
                    this.text = function () {
                        var rejected = consumed(this);
                        return rejected ? rejected : Promise.resolve(this._bodyText);
                    };
                }

                if (support.formData) {
                    this.formData = function () {
                        return this.text().then(decode);
                    };
                }

                this.json = function () {
                    return this.text().then(JSON.parse);
                };

                return this;
            } // HTTP methods whose capitalization should be normalized


            var methods = ['DELETE', 'GET', 'HEAD', 'OPTIONS', 'POST', 'PUT'];

            function normalizeMethod(method) {
                var upcased = method.toUpperCase();
                return methods.indexOf(upcased) > -1 ? upcased : method;
            }

            function Request(input, options) {
                options = options || {};
                var body = options.body;

                if (Request.prototype.isPrototypeOf(input)) {
                    if (input.bodyUsed) {
                        throw new TypeError('Already read');
                    }

                    this.url = input.url;
                    this.responseType = input.responseType;
                    this.credentials = input.credentials;

                    if (!options.headers) {
                        this.headers = new Headers(input.headers);
                    }

                    this.method = input.method;
                    this.mode = input.mode;

                    if (!body) {
                        body = input._bodyInit;
                        input.bodyUsed = true;
                    }
                } else {
                    this.url = input;
                }

                this.responseType = options.responseType || this.responseType;
                this.credentials = options.credentials || this.credentials || 'omit';

                if (options.headers || !this.headers) {
                    this.headers = new Headers(options.headers);
                }

                this.method = normalizeMethod(options.method || this.method || 'GET');
                this.mode = options.mode || this.mode || null;
                this.referrer = null;

                if ((this.method === 'GET' || this.method === 'HEAD') && body) {
                    throw new TypeError('Body not allowed for GET or HEAD requests');
                }

                this._initBody(body, options);
            }

            Request.prototype.clone = function () {
                return new Request(this);
            };

            function decode(body) {
                var form = new FormData();
                body.trim().split('&').forEach(function (bytes) {
                    if (bytes) {
                        var split = bytes.split('=');
                        var name = split.shift().replace(/\+/g, ' ');
                        var value = split.join('=').replace(/\+/g, ' ');
                        form.append(decodeURIComponent(name), decodeURIComponent(value));
                    }
                });
                return form;
            }

            function headers(xhr) {
                var head = new Headers(); // console.log(xhr._headers)
                // TODO figure out why this isn't supported
                // var pairs = xhr.getAllResponseHeaders().trim().split('\n')
                // pairs.forEach(function(header) {
                //     var split = header.trim().split(':')
                //     var key = split.shift().trim()
                //     var value = split.join(':').trim()
                //     head.append(key, value)
                // })
                // Alternative header parsing for now, using function we shouldn't use
                // for (var key in locationHeader) {
                //     if (locationHeader.hasOwnProperty(key)) {
                //         // Do things here
                //         head.append(key, locationHeader[key])
                //     }
                // }

                var locationHeader = xhr.getResponseHeader('location');

                if (locationHeader) {
                    head.append('location', locationHeader);
                }

                return head;
            }

            Body.call(Request.prototype);

            function Response(bodyInit, options) {
                if (!options) {
                    options = {};
                }

                this._initBody(bodyInit, options);

                this.type = 'default';
                this.status = options.status;
                this.ok = this.status >= 200 && this.status < 300;
                this.statusText = options.statusText;
                this.headers = options.headers instanceof Headers ? options.headers : new Headers(options.headers);
                this.url = options.url || '';
            }

            Body.call(Response.prototype);

            Response.prototype.clone = function () {
                return new Response(this._bodyInit, {
                    status: this.status,
                    statusText: this.statusText,
                    headers: new Headers(this.headers),
                    url: this.url
                });
            };

            Response.error = function () {
                var response = new Response(null, {
                    status: 0,
                    statusText: ''
                });
                response.type = 'error';
                return response;
            };

            var redirectStatuses = [301, 302, 303, 307, 308];

            Response.redirect = function (url, status) {
                if (redirectStatuses.indexOf(status) === -1) {
                    throw new RangeError('Invalid status code');
                }

                return new Response(null, {
                    status: status,
                    headers: {
                        location: url
                    }
                });
            };

            self.Headers = Headers;
            self.Request = Request;
            self.Response = Response;

            self.fetch = function (input, init) {
                return new Promise(function (resolve, reject) {
                    var request;

                    if (Request.prototype.isPrototypeOf(input) && !init) {
                        request = input;
                    } else {
                        request = new Request(input, init);
                    }

                    var xhr = new XMLHttpRequest();

                    function responseURL() {
                        if ('responseURL' in xhr) {
                            return xhr.responseURL;
                        } // TODO Figure out why this isnt supported
                        // // Avoid security warnings on getResponseHeader when not allowed by CORS
                        // if (/^X-Request-URL:/m.test(xhr.getAllResponseHeaders())) {
                        //     return xhr.getResponseHeader('X-Request-URL')
                        // }


                        return;
                    }

                    var __onLoadHandled = false;

                    function onload() {
                        if (xhr.readyState !== 4) {
                            return;
                        }

                        var status = xhr.status === 1223 ? 204 : xhr.status;

                        if (status < 100 || status > 599) {
                            if (__onLoadHandled) {
                                return;
                            } else {
                                __onLoadHandled = true;
                            }

                            reject(new TypeError('Network request failed'));
                            return;
                        }

                        var options = {
                            status: status,
                            statusText: xhr.statusText,
                            headers: headers(xhr),
                            url: responseURL()
                        };
                        var body = 'response' in xhr ? xhr.response : xhr.responseText;

                        if (__onLoadHandled) {
                            return;
                        } else {
                            __onLoadHandled = true;
                        }

                        resolve(new Response(body, options));
                    }

                    xhr.onreadystatechange = onload;
                    xhr.onload = onload;

                    xhr.onerror = function () {
                        if (__onLoadHandled) {
                            return;
                        } else {
                            __onLoadHandled = true;
                        }

                        reject(new TypeError('Network request failed'));
                    };

                    xhr.open(request.method, request.url, true); // `withCredentials` should be setted after calling `.open` in IE10
                    // http://stackoverflow.com/a/19667959/1219343

                    try {
                        if (request.credentials === 'include') {
                            // if ('withCredentials' in xhr) {
                            xhr.withCredentials = true; // } else {
                            //     console && console.warn && console.warn('withCredentials is not supported, you can ignore this warning');
                            // }
                            // console.log(`Inside fetch, here's responseType ${request.responseType}`)
                        }
                    } catch (e) {
                        console && console.warn && console.warn('set withCredentials error:' + e);
                    }

                    if ('responseType' in xhr && support.blob || request.responseType === 'blob') {
                        xhr.responseType = 'blob';
                    } // if ('responseType' in xhr && request.jsonResponseType) {
                    //     xhr.responseType = 'json'
                    // }


                    request.headers.forEach(function (value, name) {
                        xhr.setRequestHeader(name, value);
                    });
                    xhr.send(typeof request._bodyInit === 'undefined' ? null : request._bodyInit);
                });
            };

            self.fetch.polyfill = true; // Support CommonJS

            if ( module.exports) {
                module.exports = self.fetch;
            }
        })(commonjsGlobal);
    });

    var delay = function delay(ms) {
        return new Promise(function (res) {
            return setTimeout(res, ms);
        });
    };

    var MicrosoftOneDriveAPI = /*#__PURE__*/function (_LHBaseClass) {
        _inherits(MicrosoftOneDriveAPI, _LHBaseClass);

        var _super = _createSuper(MicrosoftOneDriveAPI);

        function MicrosoftOneDriveAPI(params) {
            var _this;

            _classCallCheck(this, MicrosoftOneDriveAPI);

            _this = _super.call(this, params);
            _this.accessToken = _this.getParam(params, "accessToken", null);
            _this.clientId = _this.getParam(params, "clientId", null);
            _this.clientSecret = _this.getParam(params, "clientSecret", null);
            _this.redirectUri = _this.getParam(params, "redirectUri", null);
            _this.scopes = _this.getParam(params, "scopes", null); // Part of the URL in refresh token, can probably get removed when all local tests work

            _this.tenantId = _this.getParam(params, "tenantId", null);
            _this.refreshToken = _this.getParam(params, "refreshToken", null);
            _this.baseUrl = "https://graph.microsoft.com/v1.0";
            _this.authUrl = "https://login.microsoftonline.com/common/oauth2/v2.0"; // Overall information about user's One Drive (storage, etc)

            _this.meDriveEndpoint = "/me/drive"; // Basic endpoint to recieve params - works for files and folders

            _this.fileEndpoint = function (id) {
                return "".concat(_this.meDriveEndpoint, "/items/").concat(id);
            }; // Example: /drive/root:/consequatur
            // When the path is inherited from api results, the api includes `/drive.root:/path:/..
            // TODO: Ask Sean about input format for paths/how users will get that string


            _this.pathEndpoint = function (path) {
                return "".concat(_this.meDriveEndpoint, "/root:").concat(path);
            };

            _this.URLEndpoints = {
                // Assuming the path is like /drive/root:/folder
                copy: function copy(path) {
                    return "".concat(_this.pathEndpoint(path), ":/copy");
                },
                // Trying to simplify copy methods
                copyById: function copyById(id) {
                    return "".concat(_this.fileEndpoint(id), "/copy");
                },
                getInfoById: function getInfoById(id) {
                    return _this.fileEndpoint(id);
                },
                getInfo: function getInfo(path) {
                    return _this.pathEndpoint(path);
                },
                // move: (path) => `${this.pathEndpoint(path)}:/move`,
                // this one is a weird endpoint
                // move: (path) => `${this.meDriveEndpoint}/items/root:${path}`,
                listContents: function listContents(path) {
                    return "".concat(_this.pathEndpoint(path), ":/children");
                },
                getShareUrl: function getShareUrl(path) {
                    return "".concat(_this.pathEndpoint(path), ":/createLink");
                },
                getShareUrlById: function getShareUrlById(id) {
                    return "".concat(_this.fileEndpoint(id), "/createLink");
                },
                // Assuming that parent path is inherited
                createFolder: function createFolder(path) {
                    return "".concat(_this.pathEndpoint(path), ":/children");
                },
                // createFolder: (path) => `${this.pathEndpoint(path)}:/children`,
                "delete": function _delete(path) {
                    return _this.URLEndpoints.getInfo(path);
                },
                // Example: https://graph.microsoft.com/v1.0/me/drive/root:/doloribus
                move: function move(path) {
                    return _this.pathEndpoint(path);
                },
                download: function download(path) {
                    return "".concat(_this.pathEndpoint(path), ":/content");
                },
                updateTags: function updateTags(path) {
                    return _this.URLEndpoints.getInfo(path);
                },
                upload: function upload(path) {
                    return "".concat(_this.pathEndpoint(path), ":/createUploadSession");
                },
                search: function search(query) {
                    return "".concat(_this.meDriveEndpoint, "/root/search(q='").concat(query, "')");
                },
                listRootContents: function listRootContents(path) {
                    return "".concat(_this.meDriveEndpoint, "/root/children");
                },
                batch: function batch() {
                    return "/$batch";
                }
            };
            return _this;
        }

        _createClass(MicrosoftOneDriveAPI, [{
            key: "refreshAccessToken",
            value: function () {
                var _refreshAccessToken = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee(refreshToken) {
                    var body, options, res;
                    return regeneratorRuntime.wrap(function _callee$(_context) {
                        while (1) {
                            switch (_context.prev = _context.next) {
                                case 0:
                                    body = "grant_type=refresh_token&refresh_token=".concat(refreshToken, "&client_id=").concat(this.clientId, "&client_secret=").concat(this.clientSecret, "&scope=").concat(this.scopes, "&redirect_uri=").concat(this.redirectUri);
                                    options = {
                                        method: 'POST',
                                        headers: {
                                            "Content-Type": "application/x-www-form-urlencoded"
                                        },
                                        url: "".concat(this.authUrl, "/token"),
                                        body: encodeURI(body)
                                    };
                                    _context.next = 4;
                                    return fetch(options.url, options);

                                case 4:
                                    res = _context.sent;
                                    _context.next = 7;
                                    return res.json();

                                case 7:
                                    res = _context.sent;
                                    this.setAccessToken(res.access_token);
                                    this.refreshToken = res.refresh_token;

                                case 10:
                                case "end":
                                    return _context.stop();
                            }
                        }
                    }, _callee, this);
                }));

                function refreshAccessToken(_x) {
                    return _refreshAccessToken.apply(this, arguments);
                }

                return refreshAccessToken;
            }() // For setting access token when it's returned in Oauth2

        }, {
            key: "setAccessToken",
            value: function setAccessToken(accessToken) {
                this.accessToken = accessToken;
            } // How to determine if the path is just the root, or in a folder inside the root.
            // If it is just the root, then no ":" is neccessary
            // Mostly useful for list contents

        }, {
            key: "determinePath",
            value: function determinePath(path) {
                return path === "/" || path === "root" ? // return the url endpoint that contains ':'
                    this.URLEndpoints.listRootContents(path) : // return the url endpoint that does not ^
                    this.URLEndpoints.listContents(path);
            }
        }, {
            key: "cleanPath",
            value: function cleanPath(path) {
                if (path.includes('/drive/root:')) {
                    var splitPath = path.split('/drive/root:');
                    path = splitPath[1];
                }

                return path;
            }
        }, {
            key: "updateKeys",
            value: function updateKeys(params) {
                this.clientId = this.getParam(params, "clientId", null);
                this.clientSecret = this.getParam(params, "clientSecret", null);
                this.redirectUri = this.getParam(params, "redirectUri", null);
                this.scopes = this.getParam(params, "scopes", null);
            } // injects the access token into an object and returns the headers for most api calls

        }, {
            key: "getHeaders",
            value: function getHeaders() {
                var headers = {
                    Authorization: "Bearer ".concat(this.accessToken),
                    "Content-Type": "application/json"
                };
                return headers;
            } // check the response of a fetch() before returning the data in JSON form.
            // may throw an exception if the response.status corresponds to an error

        }, {
            key: "_checkResponse",
            value: function () {
                var _checkResponse2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee2(response, url) {
                    return regeneratorRuntime.wrap(function _callee2$(_context2) {
                        while (1) {
                            switch (_context2.prev = _context2.next) {
                                case 0:
                                    if (!(response.status === 202)) {
                                        _context2.next = 2;
                                        break;
                                    }

                                    return _context2.abrupt("return", response.statusText);

                                case 2:
                                    if (!(response.status === 204)) {
                                        _context2.next = 4;
                                        break;
                                    }

                                    return _context2.abrupt("return", true);

                                case 4:
                                    if (response.status >= 400) {
                                        this.throwException("http [".concat(response.status, "] ").concat(url, ": ") + JSON.stringify(response));
                                    }

                                    _context2.prev = 5;
                                    _context2.next = 8;
                                    return response.json();

                                case 8:
                                    return _context2.abrupt("return", _context2.sent);

                                case 11:
                                    _context2.prev = 11;
                                    _context2.t0 = _context2["catch"](5);

                                    if (!(response.error === null || response.error === undefined)) {
                                        _context2.next = 15;
                                        break;
                                    }

                                    return _context2.abrupt("return", {
                                        error: null
                                    });

                                case 15:
                                    return _context2.abrupt("return", {
                                        error: JSON.stringify(response)
                                    });

                                case 16:
                                case "end":
                                    return _context2.stop();
                            }
                        }
                    }, _callee2, this, [[5, 11]]);
                }));

                function _checkResponse(_x2, _x3) {
                    return _checkResponse2.apply(this, arguments);
                }

                return _checkResponse;
            }() // route all GET requests thru this function to do error checking and return the JSON data

        }, {
            key: "_get",
            value: function () {
                var _get2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee3(apiURLending) {
                    var url, headers, response;
                    return regeneratorRuntime.wrap(function _callee3$(_context3) {
                        while (1) {
                            switch (_context3.prev = _context3.next) {
                                case 0:
                                    // let qs = new URLSearchParamsPartial(options.qs);
                                    // qs = "?" + qs.toString();
                                    url = this.baseUrl + apiURLending;
                                    headers = this.getHeaders();
                                    _context3.next = 4;
                                    return fetch(url, {
                                        method: "GET",
                                        headers: headers,
                                        credentials: "include"
                                    });

                                case 4:
                                    response = _context3.sent;
                                    _context3.next = 7;
                                    return this._checkResponse(response, url);

                                case 7:
                                    return _context3.abrupt("return", _context3.sent);

                                case 8:
                                case "end":
                                    return _context3.stop();
                            }
                        }
                    }, _callee3, this);
                }));

                function _get(_x4) {
                    return _get2.apply(this, arguments);
                }

                return _get;
            }() // route all POST requests thru this function to do error checking and return the JSON data

        }, {
            key: "_post",
            value: function () {
                var _post2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee4(apiURLEnding, data) {
                    var url, headers, response;
                    return regeneratorRuntime.wrap(function _callee4$(_context4) {
                        while (1) {
                            switch (_context4.prev = _context4.next) {
                                case 0:
                                    url = this.baseUrl + apiURLEnding;
                                    headers = this.getHeaders();
                                    _context4.next = 4;
                                    return fetch(url, {
                                        method: "POST",
                                        headers: headers,
                                        credentials: "include",
                                        body: JSON.stringify(data)
                                    });

                                case 4:
                                    response = _context4.sent;
                                    _context4.next = 7;
                                    return this._checkResponse(response, url);

                                case 7:
                                    return _context4.abrupt("return", _context4.sent);

                                case 8:
                                case "end":
                                    return _context4.stop();
                            }
                        }
                    }, _callee4, this);
                }));

                function _post(_x5, _x6) {
                    return _post2.apply(this, arguments);
                }

                return _post;
            }() // route PUT api calls thru this function for error chaecking and to return the JSON data

        }, {
            key: "_put",
            value: function () {
                var _put2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee5(apiURLEnding, data) {
                    var url, headers, response;
                    return regeneratorRuntime.wrap(function _callee5$(_context5) {
                        while (1) {
                            switch (_context5.prev = _context5.next) {
                                case 0:
                                    url = this.baseUrl + apiURLEnding;
                                    headers = this.getHeaders();
                                    _context5.next = 4;
                                    return fetch(url, {
                                        method: "PUT",
                                        headers: headers,
                                        credentials: "include",
                                        body: JSON.stringify(data)
                                    });

                                case 4:
                                    response = _context5.sent;
                                    _context5.next = 7;
                                    return this._checkResponse(response, url);

                                case 7:
                                    return _context5.abrupt("return", _context5.sent);

                                case 8:
                                case "end":
                                    return _context5.stop();
                            }
                        }
                    }, _callee5, this);
                }));

                function _put(_x7, _x8) {
                    return _put2.apply(this, arguments);
                }

                return _put;
            }() // TODO: Finish for upload file
            // Different than typical put request, used for 'uploadFile'
            // Info: https://docs.microsoft.com/en-us/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#example

        }, {
            key: "_put_upload",
            value: function () {
                var _put_upload2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee6(uploadUrl, file) {
                    var url, startBytes, endBytes, totalBytes, contentLength, rangeKeys, headers, response;
                    return regeneratorRuntime.wrap(function _callee6$(_context6) {
                        while (1) {
                            switch (_context6.prev = _context6.next) {
                                case 0:
                                    // Make sure we have what we need
                                    if (!uploadUrl) {
                                        this.throwException(uploadUrl);
                                    }

                                    if (!file) {
                                        this.throwException(file);
                                    }

                                    url = uploadUrl; // example.png file input object -- unit is 'bytes'

                                    /*
                  const file = {
                    total: 128
                    range: {
                      start: 0,
                      end: 25
                    },
                    // Assuming the file content will be attached byte by byte
                    content: {
                      1: kjakdkafjldf,
                      2: alkdsjflkadsf,
                      3: lkdajfklajdsf,
                      etc...
                    }
                  }
                  */
                                    // Will be 0 on first session

                                    startBytes = file.range.start; // Number of bytes to stop at

                                    endBytes = file.range.end; // Total bytes

                                    totalBytes = file.total; // Function that produces a new array of all the keys which have values being uploaded.
                                    // TODO: Map out values
                                    // Add 1 to the length of whatever the range is
                                    // TODO: Not sure if this will work on the final upload session

                                    contentLength = endBytes + 1; // Loop through what will be uploaded in this session alone

                                    rangeKeys = function rangeKeys(start, stop) {
                                        var step = arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : 1;
                                        return Array(Math.ceil((stop - start) / step)).fill(start).map(function (x, y) {
                                            return x + y * step;
                                        });
                                    };

                                    console.log(rangeKeys(startByte, endByte)); // That data from each of the keys values is added as the body in the request
                                    // const data = //TODO
                                    // Example:
                                    // Content-Length: 26
                                    // Content-Range: bytes 0-25/128
                                    // <bytes 0-25 of the file>

                                    headers = {
                                        Authorization: "Bearer ".concat(this.accessToken),
                                        // "Content-Type": "application/json"
                                        "Content-Length": contentLength,
                                        "Content-Range": "bytes ".concat(startBytes, "-").concat(endBytes, "/").concat(totalBytes)
                                    };
                                    _context6.next = 12;
                                    return fetch(url, {
                                        method: "PUT",
                                        headers: headers,
                                        credentials: "include",
                                        body: data
                                    });

                                case 12:
                                    response = _context6.sent;
                                    _context6.next = 15;
                                    return this._checkResponse(response, url);

                                case 15:
                                    return _context6.abrupt("return", _context6.sent);

                                case 16:
                                case "end":
                                    return _context6.stop();
                            }
                        }
                    }, _callee6, this);
                }));

                function _put_upload(_x9, _x10) {
                    return _put_upload2.apply(this, arguments);
                }

                return _put_upload;
            }() // route all DELETE api calls thru this function for error checking and return JSON data

        }, {
            key: "_delete",
            value: function () {
                var _delete2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee7(apiURLEnding) {
                    var url, headers, response;
                    return regeneratorRuntime.wrap(function _callee7$(_context7) {
                        while (1) {
                            switch (_context7.prev = _context7.next) {
                                case 0:
                                    url = this.baseUrl + apiURLEnding;
                                    headers = this.getHeaders();
                                    _context7.next = 4;
                                    return fetch(url, {
                                        method: "DELETE",
                                        headers: headers,
                                        credentials: "include"
                                    });

                                case 4:
                                    response = _context7.sent;
                                    _context7.next = 7;
                                    return this._checkResponse(response, url);

                                case 7:
                                    return _context7.abrupt("return", _context7.sent);

                                case 8:
                                case "end":
                                    return _context7.stop();
                            }
                        }
                    }, _callee7, this);
                }));

                function _delete(_x11) {
                    return _delete2.apply(this, arguments);
                }

                return _delete;
            }() // route PATCH api calls thru this function for error chaecking and to return the JSON data

        }, {
            key: "_patch",
            value: function () {
                var _patch2 = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee8(apiURLEnding, data) {
                    var url, headers, response;
                    return regeneratorRuntime.wrap(function _callee8$(_context8) {
                        while (1) {
                            switch (_context8.prev = _context8.next) {
                                case 0:
                                    url = this.baseUrl + apiURLEnding;
                                    headers = this.getHeaders();
                                    _context8.next = 4;
                                    return fetch(url, {
                                        method: "PATCH",
                                        headers: headers,
                                        credentials: "include",
                                        body: JSON.stringify(data)
                                    });

                                case 4:
                                    response = _context8.sent;
                                    _context8.next = 7;
                                    return this._checkResponse(response, url);

                                case 7:
                                    return _context8.abrupt("return", _context8.sent);

                                case 8:
                                case "end":
                                    return _context8.stop();
                            }
                        }
                    }, _callee8, this);
                }));

                function _patch(_x12, _x13) {
                    return _patch2.apply(this, arguments);
                }

                return _patch;
            }() // Search users OneDrive/root for a keyword, added as 'q' to params

        }, {
            key: "searchDrive",
            value: function () {
                var _searchDrive = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee9(query) {
                    var urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee9$(_context9) {
                        while (1) {
                            switch (_context9.prev = _context9.next) {
                                case 0:
                                    if (!query) {
                                        this.throwException("query not specified");
                                    }

                                    urlEndpoint = this.URLEndpoints.search(query);
                                    _context9.next = 4;
                                    return this._get(urlEndpoint);

                                case 4:
                                    return _context9.abrupt("return", _context9.sent);

                                case 5:
                                case "end":
                                    return _context9.stop();
                            }
                        }
                    }, _callee9, this);
                }));

                function searchDrive(_x14) {
                    return _searchDrive.apply(this, arguments);
                }

                return searchDrive;
            }() // list the items in a folder. specify the folderId of the folder you want to list the items for

        }, {
            key: "listFolderContentsByPath",
            value: function () {
                var _listFolderContentsByPath = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee10(path) {
                    var urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee10$(_context10) {
                        while (1) {
                            switch (_context10.prev = _context10.next) {
                                case 0:
                                    if (!path) {
                                        this.throwException("path not specified");
                                    } // Check if it's a folder that's not root itself
                                    //


                                    urlEndpoint = this.determinePath(path);
                                    _context10.next = 4;
                                    return this._get(urlEndpoint);

                                case 4:
                                    return _context10.abrupt("return", _context10.sent);

                                case 5:
                                case "end":
                                    return _context10.stop();
                            }
                        }
                    }, _callee10, this);
                }));

                function listFolderContentsByPath(_x15) {
                    return _listFolderContentsByPath.apply(this, arguments);
                }

                return listFolderContentsByPath;
            }() // Creates a new empty folder within the specified parent folder.
            // if a folder with the same name exists in the destination, a new renamed folder will be created instead

        }, {
            key: "createFolder",
            value: function () {
                var _createFolder = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee11(newFolderName, destFolderPath) {
                    var urlEndpoint, body;
                    return regeneratorRuntime.wrap(function _callee11$(_context11) {
                        while (1) {
                            switch (_context11.prev = _context11.next) {
                                case 0:
                                    if (!newFolderName) {
                                        this.throwException("newFolderName must be specified");
                                    }

                                    if (destFolderPath === undefined || !destFolderPath) {
                                        this.throwException("destFolderPath must be specified");
                                    } // let urlEndpoint = this.fileEndpoint + `/${destFolderPath}/children`;
                                    // Anything after 'root' will need to be added here
                                    // Example: root:/folder => path = folder
                                    // root:/folder/another-folder/yet-another-folder => path = folder/another-folder/yet-another-folder
                                    // Info: https://docs.microsoft.com/en-us/graph/api/resources/onedrive?view=graph-rest-1.0#commonly-accessed-resources


                                    if (destFolderPath == '/') {
                                        urlEndpoint = "".concat(this.meDriveEndpoint, "/root/children");
                                    } else {
                                        urlEndpoint = this.URLEndpoints.createFolder(destFolderPath);
                                    }

                                    body = {
                                        name: newFolderName,
                                        folder: {},
                                        "@microsoft.graph.conflictBehavior": "rename"
                                    };
                                    console.log(urlEndpoint);
                                    _context11.next = 7;
                                    return this._post(urlEndpoint, body);

                                case 7:
                                    return _context11.abrupt("return", _context11.sent);

                                case 8:
                                case "end":
                                    return _context11.stop();
                            }
                        }
                    }, _callee11, this);
                }));

                function createFolder(_x16, _x17) {
                    return _createFolder.apply(this, arguments);
                }

                return createFolder;
            }() //  Works for both folder and file
            // Creates a copy of a folder within a destination folder.

        }, {
            key: "copy",
            value: function () {
                var _copy = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee13(sourcePath, destFolderPath) {
                    var _this2 = this;

                    var body, urlEndpoint, initialUrl, headers, initialRes, processEndpoint, checkStatus;
                    return regeneratorRuntime.wrap(function _callee13$(_context13) {
                        while (1) {
                            switch (_context13.prev = _context13.next) {
                                case 0:
                                    if (!sourcePath) {
                                        this.throwException("folder or file path not specified");
                                    }

                                    if (!destFolderPath) {
                                        this.throwException("destFolderPath not specified");
                                    } // Get id of dest path first
                                    // let res = await this.getInfo(destFolderPath);
                                    //
                                    // And for object's path
                                    // let resTwo = await this.getInfo(sourcePath);
                                    // let destId = res.id;
                                    // let sourceId = resTwo.id;


                                    sourcePath = this.cleanPath(sourcePath);
                                    body = {
                                        parentReference: {
                                            path: destFolderPath
                                        } // "@microsoft.graph.conflictBehavior": "rename"

                                    };
                                    urlEndpoint = "".concat(this.pathEndpoint(sourcePath), ":/copy");
                                    initialUrl = this.baseUrl + urlEndpoint;
                                    headers = this.getHeaders();
                                    _context13.next = 9;
                                    return fetch(initialUrl, {
                                        method: "POST",
                                        headers: headers,
                                        credentials: "include",
                                        body: JSON.stringify(body)
                                    });

                                case 9:
                                    initialRes = _context13.sent;
                                    _context13.next = 12;
                                    return this._checkResponse(initialRes, initialUrl);

                                case 12:
                                    processEndpoint = initialRes.headers.get('Location');

                                    checkStatus = /*#__PURE__*/function () {
                                        var _ref = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee12(statusEndpoint) {
                                            var processStatusResponse, check, fullInfo;
                                            return regeneratorRuntime.wrap(function _callee12$(_context12) {
                                                while (1) {
                                                    switch (_context12.prev = _context12.next) {
                                                        case 0:
                                                            _context12.next = 2;
                                                            return fetch(processEndpoint);

                                                        case 2:
                                                            processStatusResponse = _context12.sent;
                                                            _context12.next = 5;
                                                            return processStatusResponse.json();

                                                        case 5:
                                                            check = _context12.sent;

                                                            if (!(check.status == 'failed')) {
                                                                _context12.next = 10;
                                                                break;
                                                            }

                                                            _this2.throwException("Copy folder or file failed with error: ".concat(check.error.message));

                                                            _context12.next = 26;
                                                            break;

                                                        case 10:
                                                            if (!(check.status === 'notStarted' || check.status === 'inProgress')) {
                                                                _context12.next = 18;
                                                                break;
                                                            }

                                                            _context12.next = 13;
                                                            return delay(5000);

                                                        case 13:
                                                            _context12.next = 15;
                                                            return checkStatus(statusEndpoint);

                                                        case 15:
                                                            return _context12.abrupt("return", _context12.sent);

                                                        case 18:
                                                            if (!(check.status === 'completed')) {
                                                                _context12.next = 25;
                                                                break;
                                                            }

                                                            _context12.next = 21;
                                                            return _this2.getInfoById(check.resourceId);

                                                        case 21:
                                                            fullInfo = _context12.sent;
                                                            return _context12.abrupt("return", fullInfo);

                                                        case 25:
                                                            _this2.throwException("Copy folder failed with unknown error: ".concat(JSON.stringify(check)));

                                                        case 26:
                                                        case "end":
                                                            return _context12.stop();
                                                    }
                                                }
                                            }, _callee12);
                                        }));

                                        return function checkStatus(_x20) {
                                            return _ref.apply(this, arguments);
                                        };
                                    }();

                                    _context13.next = 16;
                                    return checkStatus(processEndpoint);

                                case 16:
                                    return _context13.abrupt("return", _context13.sent);

                                case 17:
                                case "end":
                                    return _context13.stop();
                            }
                        }
                    }, _callee13, this);
                }));

                function copy(_x18, _x19) {
                    return _copy.apply(this, arguments);
                }

                return copy;
            }() // Deletes a file or folder by its path

        }, {
            key: "deleteFileOrFolder",
            value: function () {
                var _deleteFileOrFolder = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee14(path) {
                    var urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee14$(_context14) {
                        while (1) {
                            switch (_context14.prev = _context14.next) {
                                case 0:
                                    if (!path) {
                                        this.throwException("folder or file path not specified");
                                    }

                                    path = this.cleanPath(path);
                                    urlEndpoint = this.URLEndpoints["delete"](path);
                                    _context14.next = 5;
                                    return this._delete(urlEndpoint);

                                case 5:
                                    return _context14.abrupt("return", _context14.sent);

                                case 6:
                                case "end":
                                    return _context14.stop();
                            }
                        }
                    }, _callee14, this);
                }));

                function deleteFileOrFolder(_x21) {
                    return _deleteFileOrFolder.apply(this, arguments);
                }

                return deleteFileOrFolder;
            }() // Creates a shareable link, can be customized by type and scope for intended recipient
            // Info: https://docs.microsoft.com/en-us/graph/api/driveitem-createlink?view=graph-rest-1.0&tabs=http#http-request

        }, {
            key: "getShareUrlById",
            value: function () {
                var _getShareUrlById = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee15(id) {
                    var body, urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee15$(_context15) {
                        while (1) {
                            switch (_context15.prev = _context15.next) {
                                case 0:
                                    if (!id) {
                                        this.throwException("folder or file Id was not specified");
                                    }

                                    body = {
                                        type: "view",
                                        scope: "anonymous"
                                    };
                                    urlEndpoint = this.URLEndpoints.getShareUrlById(id);
                                    _context15.next = 5;
                                    return this._post(urlEndpoint, body);

                                case 5:
                                    return _context15.abrupt("return", _context15.sent);

                                case 6:
                                case "end":
                                    return _context15.stop();
                            }
                        }
                    }, _callee15, this);
                }));

                function getShareUrlById(_x22) {
                    return _getShareUrlById.apply(this, arguments);
                }

                return getShareUrlById;
            }() // Get share url by path

        }, {
            key: "getShareUrl",
            value: function () {
                var _getShareUrl = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee16(path) {
                    var body, urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee16$(_context16) {
                        while (1) {
                            switch (_context16.prev = _context16.next) {
                                case 0:
                                    if (!path) {
                                        this.throwException("folder or file path was not specified");
                                    }

                                    path = this.cleanPath(path);
                                    body = {
                                        type: "view",
                                        scope: "anonymous"
                                    };
                                    urlEndpoint = this.URLEndpoints.getShareUrl(path);
                                    _context16.next = 6;
                                    return this._post(urlEndpoint, body);

                                case 6:
                                    return _context16.abrupt("return", _context16.sent);

                                case 7:
                                case "end":
                                    return _context16.stop();
                            }
                        }
                    }, _callee16, this);
                }));

                function getShareUrl(_x23) {
                    return _getShareUrl.apply(this, arguments);
                }

                return getShareUrl;
            }() // get all information of items in a path

        }, {
            key: "getInfo",
            value: function () {
                var _getInfo = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee17(path) {
                    var urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee17$(_context17) {
                        while (1) {
                            switch (_context17.prev = _context17.next) {
                                case 0:
                                    if (!path) {
                                        this.throwException("path not specified");
                                    }

                                    path = this.cleanPath(path); // path must start with '/'

                                    console.log("get info for an item", path);
                                    urlEndpoint = this.URLEndpoints.getInfo(path);
                                    _context17.next = 6;
                                    return this._get(urlEndpoint);

                                case 6:
                                    return _context17.abrupt("return", _context17.sent);

                                case 7:
                                case "end":
                                    return _context17.stop();
                            }
                        }
                    }, _callee17, this);
                }));

                function getInfo(_x24) {
                    return _getInfo.apply(this, arguments);
                }

                return getInfo;
            }() // Get all information about a given file or folder

        }, {
            key: "getInfoById",
            value: function () {
                var _getInfoById = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee18(id, fieldSelectCSV) {
                    var urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee18$(_context18) {
                        while (1) {
                            switch (_context18.prev = _context18.next) {
                                case 0:
                                    if (!id) {
                                        this.throwException("folder or file Id was not specified");
                                    }

                                    urlEndpoint = this.URLEndpoints.getInfoById(id);

                                    if (fieldSelectCSV) {
                                        urlEndpoint += "?select=".concat(fieldSelectCSV);
                                    }

                                    _context18.next = 5;
                                    return this._get(urlEndpoint);

                                case 5:
                                    return _context18.abrupt("return", _context18.sent);

                                case 6:
                                case "end":
                                    return _context18.stop();
                            }
                        }
                    }, _callee18, this);
                }));

                function getInfoById(_x25, _x26) {
                    return _getInfoById.apply(this, arguments);
                }

                return getInfoById;
            }() // Make a Batch request to retrieve bulk data

        }, {
            key: "batchRequest",
            value: function () {
                var _batchRequest = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee19(batchItems) {
                    var urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee19$(_context19) {
                        while (1) {
                            switch (_context19.prev = _context19.next) {
                                case 0:
                                    if (!batchItems) {
                                        this.throwException("batchItems must be provided");
                                    }

                                    urlEndpoint = this.URLEndpoints.batch(); // Need logic for if there are more than 20 batch items... :-)

                                    _context19.next = 4;
                                    return this._post(urlEndpoint, {
                                        requests: batchItems
                                    });

                                case 4:
                                    return _context19.abrupt("return", _context19.sent);

                                case 5:
                                case "end":
                                    return _context19.stop();
                            }
                        }
                    }, _callee19, this);
                }));

                function batchRequest(_x27) {
                    return _batchRequest.apply(this, arguments);
                }

                return batchRequest;
            }() // Move a file or folder to a new parent reference

        }, {
            key: "moveFileOrFolder",
            value: function () {
                var _moveFileOrFolder = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee20(path, destFolderPath) {
                    var body, urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee20$(_context20) {
                        while (1) {
                            switch (_context20.prev = _context20.next) {
                                case 0:
                                    if (!path) {
                                        this.throwException("folder or file path not specified");
                                    }

                                    body = {
                                        parentReference: {
                                            // 		"path": "/drive/root:"
                                            path: destFolderPath
                                        }
                                    };
                                    console.log(body); // /me/drive/root:/doloribus

                                    path = this.cleanPath(path);
                                    urlEndpoint = this.URLEndpoints.move(path);
                                    _context20.next = 7;
                                    return this._patch(urlEndpoint, body);

                                case 7:
                                    return _context20.abrupt("return", _context20.sent);

                                case 8:
                                case "end":
                                    return _context20.stop();
                            }
                        }
                    }, _callee20, this);
                }));

                function moveFileOrFolder(_x28, _x29) {
                    return _moveFileOrFolder.apply(this, arguments);
                }

                return moveFileOrFolder;
            }() // Successful response redirects to @microsoft.graph.downloadUrl property
            // Info: https://docs.microsoft.com/en-us/graph/api/driveitem-get-content?view=graph-rest-1.0&tabs=http

        }, {
            key: "downloadFile",
            value: function () {
                var _downloadFile = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee21(path) {
                    var urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee21$(_context21) {
                        while (1) {
                            switch (_context21.prev = _context21.next) {
                                case 0:
                                    if (!path) {
                                        this.throwException("path not specified");
                                    }

                                    urlEndpoint = this.URLEndpoints.download(path);
                                    _context21.next = 4;
                                    return this._get(urlEndpoint);

                                case 4:
                                    return _context21.abrupt("return", _context21.sent);

                                case 5:
                                case "end":
                                    return _context21.stop();
                            }
                        }
                    }, _callee21, this);
                }));

                function downloadFile(_x30) {
                    return _downloadFile.apply(this, arguments);
                }

                return downloadFile;
            }() // TODO: Test with different types of upload formats
            // Info: https://docs.microsoft.com/en-us/graph/api/driveitem-createuploadsession?view=graph-rest-1.0
            // This is based on Google Drive's method

        }, {
            key: "uploadFile",
            value: function () {
                var _uploadFile = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee22( // TODO: file can probably just be one object
                    fileName, fileType, destinationFolderId, fileInfo) {
                    var metadata, postEndpoint, firstRes, uploadUrl, secondRes;
                    return regeneratorRuntime.wrap(function _callee22$(_context22) {
                        while (1) {
                            switch (_context22.prev = _context22.next) {
                                case 0:
                                    if (!fileName) {
                                        this.throwException("fileName was not specified");
                                    }

                                    if (!fileType) {
                                        this.throwException("fileType was not specified");
                                    }

                                    if (!destinationFolderId) {
                                        this.throwException("destinationFolderId was not specified");
                                    } // Customize as neccessary
                                    // TODO: Try with different extensions


                                    metadata = {
                                        name: "".concat(fileName, ".txt"),
                                        item: {
                                            "@microsoft.graph.conflictBehavior": "rename"
                                        }
                                    }; // First request to open space for uploading data
                                    // Info: https://docs.microsoft.com/en-us/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#properties

                                    postEndpoint = this.URLEndpoints.upload(destinationFolderId);
                                    _context22.next = 7;
                                    return this._post(postEndpoint, metadata);

                                case 7:
                                    firstRes = _context22.sent;
                                    // console.log("upload file body, part 1:", firstRes);
                                    // Handle response and make new request with the returned url
                                    // Info: https://docs.microsoft.com/en-us/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#response
                                    // More info: https://docs.microsoft.com/en-us/graph/api/resources/uploadsession?view=graph-rest-1.0#json-representation
                                    // Example of returned body:
                                    // {
                                    //   "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
                                    //   "expirationDateTime": "2021-01-29T09:21:55.523Z"
                                    // }
                                    uploadUrl = firstRes.uploadUrl; // Make sure we have what we need

                                    if (!uploadUrl) {
                                        this.throwException("First part of upload session failed - no upload url provdided");
                                    } // Make a 'put' request to uploadUrl to begin uploading bytes
                                    // Info: https://docs.microsoft.com/en-us/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#upload-bytes-to-the-upload-session
                                    // Content length, range, and content must be included
                                    // Brought in as 'file' object
                                    // console.log("file info", file);


                                    if (!file.content) {
                                        this.throwException("file content not specified");
                                    } // Length means the number of bytes being uploaded in this session alone
                                    // if (!file.length) {
                                    //   this.throwException('file length not specified')
                                    // }
                                    // Range is the ratio of bytes uploaded in this session to total bytes in the file


                                    if (!file.range) {
                                        this.throwException;
                                    }

                                    _context22.next = 14;
                                    return this._put_upload(uploadUrl);

                                case 14:
                                    secondRes = _context22.sent;

                                case 15:
                                case "end":
                                    return _context22.stop();
                            }
                        }
                    }, _callee22, this);
                }));

                function uploadFile(_x31, _x32, _x33, _x34) {
                    return _uploadFile.apply(this, arguments);
                }

                return uploadFile;
            }() // Get information about user's drive

        }, {
            key: "getServiceQuota",
            value: function () {
                var _getServiceQuota = _asyncToGenerator( /*#__PURE__*/regeneratorRuntime.mark(function _callee23() {
                    var urlEndpoint;
                    return regeneratorRuntime.wrap(function _callee23$(_context23) {
                        while (1) {
                            switch (_context23.prev = _context23.next) {
                                case 0:
                                    urlEndpoint = this.meDriveEndpoint;
                                    _context23.next = 3;
                                    return this._get(urlEndpoint);

                                case 3:
                                    return _context23.abrupt("return", _context23.sent);

                                case 4:
                                case "end":
                                    return _context23.stop();
                            }
                        }
                    }, _callee23, this);
                }));

                function getServiceQuota() {
                    return _getServiceQuota.apply(this, arguments);
                }

                return getServiceQuota;
            }()
        }]);

        return MicrosoftOneDriveAPI;
    }(LHBaseClass_1);

    var MicrosoftOneDriveAPI_1 = MicrosoftOneDriveAPI;

    var Integration = /*#__PURE__*/function (_K2BaseIntegration) {
        _inherits(Integration, _K2BaseIntegration);

        var _super = _createSuper(Integration);

        function Integration(params) {
            var _this;

            _classCallCheck(this, Integration);

            _this = _super.call(this, params);
            _this.metaData = {
                systemName: "MicrosoftOneDriveIntegration",
                displayName: "Microsoft OneDrive Integration",
                description: "Integration of Microsoft OneDrive"
            };
            _this.api = new MicrosoftOneDriveAPI_1();
            var soParams = {
                api: _this.api
            };
            _this.smartObjects = [new File_1(soParams), new Folder_1(soParams), new Service_1(soParams)];
            return _this;
        }

        _createClass(Integration, [{
            key: "getMetaData",
            value: function getMetaData() {
                return this.metaData;
            }
        }]);

        return Integration;
    }(K2BaseIntegration_1);

    var Integration_1 = Integration;

    integration = new Integration_1();
    metadata = integration.getMetaData();

    ondescribe = function ondescribe(_ref) {
        var configuration = _ref.configuration;
        postSchema(integration.getSchemas());
    };

    onexecute = function onexecute(_ref2) {
        var objectName = _ref2.objectName,
            methodName = _ref2.methodName,
            parameters = _ref2.parameters,
            properties = _ref2.properties;
        return integration.execute(objectName, methodName, parameters, properties);
    };

    setTimeout = function setTimeout(callback, ms) {

        callback();
    };

}());
//# sourceMappingURL=index.js.map